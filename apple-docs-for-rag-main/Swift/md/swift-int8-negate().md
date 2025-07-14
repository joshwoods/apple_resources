

- Swift
- Int8
-  negate() 

Instance Method

# negate()

Replaces this value with its additive inverse.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func negate()
```

## Discussion

The following example uses the `negate()` method to negate the value of an integer `x`:

```
var x = 21
x.negate()
// x == -21
```

The resulting value must be representable within the value’s type. In particular, negating a signed, fixed-width integer type’s minimum results in a value that cannot be represented.

```
var y = Int8.min
y.negate()
// Overflow error
```

