##Learning Ruby - Fibonacci (Euler Question 2)

I attempted this question to practice my grasp in arrays, which has been my weakest point at the time of this task.

This question can be found on [Project Euler](http://projecteuler.net/problem=2).

(Week 2)

###Question:
Each new term in the Fibonacci sequence is generated by adding the previous two terms. By starting with 1 and 2, the first 10 terms will be:

1, 2, 3, 5, 8, 13, 21, 34, 55, 89, ...

By considering the terms in the Fibonacci sequence whose values do not exceed four million, find the sum of the even-valued terms.


###My Solution:
```ruby
arr = [1,1]
while arr[-1]<=4000000
arr << arr[-1]+arr[-2]
end
even_fib = arr.select {|x| x%2==0}
puts even_fib.inject(:+)


```
##Technologies Used
- Ruby
