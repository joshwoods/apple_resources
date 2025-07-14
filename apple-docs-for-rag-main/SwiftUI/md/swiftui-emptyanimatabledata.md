

- SwiftUI
-  EmptyAnimatableData 

Structure

# EmptyAnimatableData

An empty type for animatable data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct EmptyAnimatableData
```

## Overview

This type is suitable for use as the `animatableData` property of types that do not have any animatable properties.

## Topics

### Creating the data

init()

### Manipulating the data

var magnitudeSquared: Double

The dot-product of this animatable data instance with itself.

## Relationships

### Conforms To

- AdditiveArithmetic
- BitwiseCopyable
- Copyable
- Equatable
- Sendable
- VectorArithmetic

## See Also

### Making data animatable

protocol Animatable

A type that describes how to animate a property of a view.

struct AnimatablePair

A pair of animatable values, which is itself animatable.

protocol VectorArithmetic

A type that can serve as the animatable data of an animatable type.

