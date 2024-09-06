# Pattern matching

If you set value as function argument, it become pattern It only call when passed argument is matched.
```
fact 0 = 1;
```
If you set normal symbol as function argument. It call any case without configured pattern.

```
fact n = * n (fact (- n 1))
```
