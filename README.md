There are three prompts on this assessment. The first prompt, difference, is mostly complete, but there is at least one small error that must be corrected before it has complete functionality. 

The other two prompts must be completed. Use the provided description and examples to implement the functions.

Please write down your Path of Inquiry while completing this assessment. This should consist of 2-5 bullets per prompt that describe the questions you asked yourself while working through the prompt. For example, when solving nth Fibonacci:

How do I produce a Fibonacci sequence?
- Start a sequence with the numbers 0 & 1. Add the previous two numbers to produce the next number

What data structure will I use to hold my sequence?
- I will create an array with 0 & 1.

How will I output the nth Fibonacci number?
- Make a for-loop that starts at 2 and stops at n. With each iteration, push
the sum of the values at the previous two indexes. Return the value at the nth index

Code for nthFibonacci
```javascript
function nthFibonacci(n) {
  var sequence = [0, 1];

  for (var i = 2; i <= n; i++) {
      sequence.push(sequence[i-1] + sequence[i-2]);
  }

  return sequence[n-1];
}
```