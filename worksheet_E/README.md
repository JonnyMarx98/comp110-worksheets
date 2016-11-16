a)
~~~
s2 = 0
s3 = s0
while s3 != 0:
  s2 += s1
  s3 -= 1
~~~

b)
~~~
s3 equals s0 so it will go through the loop s0 number of times because each time the loops is executed s3 decrements by 1. Each time the loop executes s1 is also added to s2 (which starts on 0), therefore it will add s1 to s2 s0 number of times. For example if s0 = 3 and s1 = 2, 2 will be added to s2 3 times which will be 6, the same as 3*2.  
~~~

c)
~~~
s0 = 10
s1 = 1
while s0 != 0:
  s2 = 0
  s3 = s0
  while s3 != 0:
    s2 += s1
    s3 -= 1
  s1 = s2
  s0 -= 1
~~~

d) 
~~~
The outer loop runs s0 number of times because s0 is decremented by 1 in each iteration of the loop until it equals 0. 
The inner loop runs s3 number of times. s3 is assigned to the value of s0 each time the outer loop runs. This means that everytime time the outer loop runs the inner loop will run 1 less time. Each time the inner loop runs it adds s1 to s2 (which is set to 0 before the inner loop) then after the inner loop s1 is assigned to the value of s2. this means that s1 = s1(s0-n) where n is the number of times the outer loop has run. so when s1 = 1, once the outer loop has finished s1 = 1(s0-0)(s0-1)(s0-2)(s0-3)(s0-4)...(s0-(s0-1)) where s0 is what s0 was at the start.
So if s0 = 10 then at the end of the outer loop:
s1 = 1(10)(10-1)(10-2)(10-3)(10-4)10-5)(10-6)(10-7)(10-8)(10-9)
which is equal to:
(10)(9)(8)(7)(6)(5)(4)(3)(2)(1)
therefore s1 = 10!
~~~

e)
~~~
addi $s0, $zero, 10
addi $s1, $zero, 1

loop:
mult $s0, $s1
mflo $s2
addi $s0, $s0, -1
addi $s1, $s2, 0
bne, $s0, $zero, loop
~~~
