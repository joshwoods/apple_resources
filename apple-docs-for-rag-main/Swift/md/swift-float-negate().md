

- Swift
- Float
-  negate() 

Instance Method

# negate()

Replaces this value with its additive inverse.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

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

## See Also

### Performing Calculations

Floating-Point Operators for Float

Perform arithmetic and bitwise operations or compare values.

func addingProduct(Self, Self) -> Self

Returns the result of adding the product of the two given values to this value, computed without intermediate rounding.

func addProduct(Float, Float)

Adds the product of the two given values to this value in place, computed without intermediate rounding.

func squareRoot() -> Self

Returns the square root of the value, rounded to a representable value.

func formSquareRoot()

Replaces this value with its square root, rounded to a representable value.

func remainder(dividingBy: Self) -> Self

Returns the remainder of this value divided by the given value.

func formRemainder(dividingBy: Float)

Replaces this value with the remainder of itself divided by the given value.

func truncatingRemainder(dividingBy: Self) -> Self

Returns the remainder of this value divided by the given value using truncating division.

func formTruncatingRemainder(dividingBy: Float)

Replaces this value with the remainder of itself divided by the given value using truncating division.

