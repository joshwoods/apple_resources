

- Swift
- FloatingPoint
-  negate() 

Instance Method

# negate()

Replaces this value with its additive inverse.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
override mutating func negate()
```

**Required**

## Discussion

The result is always exact. This example uses the `negate()` method to negate the value of the variable `x`:

```
var x = 21.5
x.negate()
// x == -21.5
```

