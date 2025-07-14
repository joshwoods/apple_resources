

- SwiftUI
- VectorArithmetic
-  interpolate(towards:amount:) 

Instance Method

# interpolate(towards:amount:)

Interpolates this value with `other` by the specified `amount`.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
mutating func interpolate(
    towards other: Self,
    amount: Double
)
```

## Discussion

This is equivalent to `self = self + (other - self) * amount`.

## See Also

### Manipulating values

var magnitudeSquared: Double

Returns the dot-product of this vector arithmetic instance with itself.

**Required**

func scale(by: Double)

Multiplies each component of this value by the given value.

**Required** Default implementation provided.

func scaled(by: Double) -> Self

Returns a value with each component of this value multiplied by the given value.

func interpolated(towards: Self, amount: Double) -> Self

Returns this value interpolated with `other` by the specified `amount`.

