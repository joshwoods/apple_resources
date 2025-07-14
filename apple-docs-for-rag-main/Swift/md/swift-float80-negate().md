

- Swift
- Float80
-  negate() 

Instance Method

# negate()

Replaces this value with its additive inverse.

macOS 10.10+

``` source
mutating func negate()
```

## Discussion

The result is always exact. This example uses the `negate()` method to negate the value of the variable `x`:

```
var x = 21.5
x.negate()
// x == -21.5
```

