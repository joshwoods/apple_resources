

- SwiftUI
-  RotatedShape 

Structure

# RotatedShape

A shape with a rotation transform applied to it.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct RotatedShape where Content : Shape
```

## Topics

### Creating a rotated shape

init(shape: Content, angle: Angle, anchor: UnitPoint)

### Getting the shape’s characteristics

var anchor: UnitPoint

var angle: Angle

var shape: Content

### Supporting types

var animatableData: RotatedShape&lt;Content>.AnimatableData

The data to animate.

## Relationships

### Conforms To

- Animatable
- Copyable
- InsettableShape

  Conforms when `Content` conforms to `InsettableShape`.

- Sendable
- Shape
- View

  Conforms when `Content` conforms to `InsettableShape`.

## See Also

### Transforming a shape

struct ScaledShape

A shape with a scale transform applied to it.

struct OffsetShape

A shape with a translation offset transform applied to it.

struct TransformedShape

A shape with an affine transform applied to it.

