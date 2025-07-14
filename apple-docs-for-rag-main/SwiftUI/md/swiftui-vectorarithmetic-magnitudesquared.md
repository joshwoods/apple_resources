

- SwiftUI
- VectorArithmetic
-  magnitudeSquared 

Instance Property

# magnitudeSquared

Returns the dot-product of this vector arithmetic instance with itself.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var magnitudeSquared: Double { get }
```

**Required**

## See Also

### Manipulating values

func scale(by: Double)

Multiplies each component of this value by the given value.

**Required** Default implementation provided.

func scaled(by: Double) -> Self

Returns a value with each component of this value multiplied by the given value.

func interpolate(towards: Self, amount: Double)

Interpolates this value with `other` by the specified `amount`.

func interpolated(towards: Self, amount: Double) -> Self

Returns this value interpolated with `other` by the specified `amount`.

