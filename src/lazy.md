# Lazy evaluation
If you want to do lazy evaluation,  prefix `@` to the expression.
function `eval` to evaluate it.
```
x = @{
    + 1 (input)
};
eval x
```
It's usually used in function `if` to conditional branches.
```
for (range 100) lambda(i -> {
    i = + i 1;
    if (equal 0 (% i 15)) @{
        print "FizzBuzz";
    } @{if (equal 0 (% i 3)) @{
        print "Fizz";
    } @{if (equal 0 (% i 5)) @{
        print "Buzz";
    } @{
       print i;
    }}}
})
```
