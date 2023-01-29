# Question 1:
```js
import java.io.IOException;
import java.net.URI;

class Handler implements StringServer {
    public String stringSite(URI url) {
        String[] output = url.split("=");
            System.out.println(output[1]);
        }
    }
```
# Question 2:
The one of the bugs from lab 3 is from the code of the method _reverseInPlace_ which tries to reverse the order of the arraylist.  A failure-inducing input would be：<br>
`{1,2,3,4,5}`<br>
Howver, an input that doesn’t induce a failure would be:<br>
`{1}`<br>
Below is the screenshots of the symptoms:<br>


Below is the bug and how we fix it:
## Before:
```js
static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
  }
```
## After:
```js
  static void reverseInPlace(int[] arr) {
    int[]newArr = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      newArr[i] = arr[arr.length - i - 1];
    }
    for(int j=0; j<arr.length;j++){
      arr[j]=newArr[j];
    }
  }
```
  
 



The codeb is originally written as reversing the array one by one that means the array would change everytime when we do the reverse. For example, {1,2,3} would 
become {3,2,3}. When we want to change the last number 3 to the origianlly first number 1, the code would use the new array {3,2,3} to run the reverse code and so it 
would then result in {3,2,3} in the end since it is not using the original array. To fix the bug, we need to create a new array and put the number in the new array once
we finishing reversing and keep the original array the same so that there would not have the issue as before. 
