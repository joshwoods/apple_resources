

- SwiftUI
-  ScaledShape 

Structure

# ScaledShape

A shape with a scale transform applied to it.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct ScaledShape where Content : Shape
```

## Topics

### Creating a scaled shape

init(shape: Content, scale: CGSize, anchor: UnitPoint)

### Getting the shape’s characteristics

var anchor: UnitPoint

var scale: CGSize

var shape: Content

### Supporting types

var animatableData: ScaledShape&lt;Content>.AnimatableData

The data to animate.

## Relationships

### Conforms To

- Animatable
- Sendable
- Shape
- View

## See Also

### Transforming a shape

struct RotatedShape

A shape with a rotation transform applied to it.

struct OffsetShape

A shape with a translation offset transform applied to it.

struct TransformedShape

A shape with an affine transform applied to it.

