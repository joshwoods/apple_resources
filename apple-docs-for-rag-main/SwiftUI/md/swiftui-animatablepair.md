

- SwiftUI
-  AnimatablePair 

Structure

# AnimatablePair

A pair of animatable values, which is itself animatable.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct AnimatablePair where First : VectorArithmetic, Second : VectorArithmetic
```

## Topics

### Creating an animatable pair

init(First, Second)

Creates an animated pair with the provided values.

### Getting the constituent animations

var first: First

The first value.

var second: Second

The second value.

### Manipulating values

var magnitudeSquared: Double

The dot-product of this animated pair with itself.

## Relationships

### Conforms To

- AdditiveArithmetic
- Equatable
- Sendable
- VectorArithmetic

## See Also

### Making data animatable

protocol Animatable

A type that describes how to animate a property of a view.

protocol VectorArithmetic

A type that can serve as the animatable data of an animatable type.

struct EmptyAnimatableData

An empty type for animatable data.

