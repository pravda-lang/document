# Code block

If you surround by brace, the inside code will be block.
The last expression in the block returns value.

```
{
  b = {
    c = 1;
    + c 1
  };
  + b 1
}
```
In this code, the block returns 3. variable "b" defined in the block is not allowed to access in outside.
