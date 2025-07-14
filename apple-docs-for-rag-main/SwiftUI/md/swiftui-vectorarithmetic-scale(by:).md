

- SwiftUI
- VectorArithmetic
-  scale(by:) 

Instance Method

# scale(by:)

Multiplies each component of this value by the given value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
mutating func scale(by rhs: Double)
```

**Required** Default implementation provided.

## Default Implementations

### VectorArithmetic Implementations

func scale(by: Double)

Multiplies each component of this value by the given value.

## See Also

### Manipulating values

var magnitudeSquared: Double

Returns the dot-product of this vector arithmetic instance with itself.

**Required**

func scaled(by: Double) -> Self

Returns a value with each component of this value multiplied by the given value.

func interpolate(towards: Self, amount: Double)

Interpolates this value with `other` by the specified `amount`.

func interpolated(towards: Self, amount: Double) -> Self

Returns this value interpolated with `other` by the specified `amount`.

