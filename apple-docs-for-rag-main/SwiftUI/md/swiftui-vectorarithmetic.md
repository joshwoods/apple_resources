

- SwiftUI
-  VectorArithmetic 

Protocol

# VectorArithmetic

A type that can serve as the animatable data of an animatable type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol VectorArithmetic : AdditiveArithmetic
```

## Overview

`VectorArithmetic` extends the `AdditiveArithmetic` protocol with scalar multiplication and a way to query the vector magnitude of the value. Use this type as the `animatableData` associated type of a type that conforms to the Animatable protocol.

## Topics

### Manipulating values

var magnitudeSquared: Double

Returns the dot-product of this vector arithmetic instance with itself.

**Required**

func scale(by: Double)

Multiplies each component of this value by the given value.

**Required** Default implementation provided.

func scaled(by: Double) -> Self

Returns a value with each component of this value multiplied by the given value.

func interpolate(towards: Self, amount: Double)

Interpolates this value with `other` by the specified `amount`.

func interpolated(towards: Self, amount: Double) -> Self

Returns this value interpolated with `other` by the specified `amount`.

## Relationships

### Inherits From

- AdditiveArithmetic
- Equatable

### Conforming Types

- AnimatablePair
- EmptyAnimatableData

## See Also

### Making data animatable

protocol Animatable

A type that describes how to animate a property of a view.

struct AnimatablePair

A pair of animatable values, which is itself animatable.

struct EmptyAnimatableData

An empty type for animatable data.

