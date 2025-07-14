

- Swift
- Float16
-  negate() 

Instance Method

# negate()

Replaces this value with its additive inverse.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

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

