# Lambda expression
It starts with `lambda` or `\` and surround by parentheses.
Inside parentheses is split by `->`, after is same to function.

```
lambda(n -> * n 2)
\(n -> * n 2)
```

Lambda expression is usually used in function `map` etc in iterator.

```
map (range 10) lambda(n -> * n 2)
```
