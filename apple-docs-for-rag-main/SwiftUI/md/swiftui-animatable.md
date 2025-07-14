

- SwiftUI
-  Animatable 

Protocol

# Animatable

A type that describes how to animate a property of a view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol Animatable
```

## Topics

### Animating data

var animatableData: Self.AnimatableData

The data to animate.

**Required** Default implementations provided.

associatedtype AnimatableData : VectorArithmetic

The type defining the data to animate.

**Required**

## Relationships

### Inherited By

- AnimatableModifier
- GeometryEffect
- InsettableShape
- Layout
- Shape
- TextRenderer
- VisualEffect

### Conforming Types

- Angle
- AnyLayout
- AnyShape
- ButtonBorderShape
- Capsule
- Circle
- Color.Resolved
- ContainerRelativeShape
- EdgeInsets
- EdgeInsets3D
- Ellipse
- EmptyVisualEffect
- GridLayout
- HStackLayout
- OffsetShape

  Conforms when `Content` conforms to `InsettableShape`.

- Path
- Rectangle
- RectangleCornerRadii
- RotatedShape
- RoundedRectangle
- ScaledShape
- StrokeStyle
- TransformedShape
- UnevenRoundedRectangle
- UnitPoint
- UnitPoint3D
- VStackLayout
- ZStackLayout

## See Also

### Making data animatable

struct AnimatablePair

A pair of animatable values, which is itself animatable.

protocol VectorArithmetic

A type that can serve as the animatable data of an animatable type.

struct EmptyAnimatableData

An empty type for animatable data.

