

- SwiftUI
- VectorArithmetic
-  scaled(by:) 

Instance Method

# scaled(by:)

Returns a value with each component of this value multiplied by the given value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func scaled(by rhs: Double) -> Self
```

## See Also

### Manipulating values

var magnitudeSquared: Double

Returns the dot-product of this vector arithmetic instance with itself.

**Required**

func scale(by: Double)

Multiplies each component of this value by the given value.

**Required** Default implementation provided.

func interpolate(towards: Self, amount: Double)

Interpolates this value with `other` by the specified `amount`.

func interpolated(towards: Self, amount: Double) -> Self

Returns this value interpolated with `other` by the specified `amount`.

