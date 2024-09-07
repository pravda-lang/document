# Lazy evaluation
If you want to do lazy evaluation,  prefix `lazy` or `@` to the expression.
```
x = @{
    + 1 (input)
};
y = lazy{
    + 1 (input)
}
```

function `eval` to evaluate it.
```
eval x
```

It's usually used in function `if` to conditional branches.
Because, function `if` needs block as arguments.
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
