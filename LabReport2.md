# Lab Report #2: Servers and Bugs 
This lab report will discuss the web server, String Server, and address bugs within a code. 



## Web Server - String Server 




## Bugs: from Array Methods
The Array Methods are intended to reverse a list, however, because of bugs in the code it 
does not output the expected results. 

**The Bug**  The bug, as the before-and-after code change required to fix it (as two code blocks in Markdown)


There is a bug specifically in the "reverseInPlace" method that incorrectly changes the input array to be in reversed order: 
The bug would correctly reverse the first half of the list, but in the second half retains the same values rather than the reversed values.

```
public class ArrayExamples {

  static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
  }
 }
 ```


**Symptom**
- The symptom, as the output of running the tests (provide it as a screenshot of running JUnit with at least the two inputs above)





**Failure Inducing Input**
- A failure-inducing input for the buggy program, as a JUnit test and any associated code (write it as a code block in Markdown)



**Non-Failure Inducing Input**
- An input that doesn’t induce a failure, as a JUnit test and any associated code (write it as a code block in Markdown)



**Addressing the Bug**
Briefly describe why the fix addresses the issue.






## What I've Learned 
