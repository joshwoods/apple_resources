

- SwiftUI
-  OffsetShape 

Structure

# OffsetShape

A shape with a translation offset transform applied to it.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct OffsetShape where Content : Shape
```

## Topics

### Creating an offset shape

init(shape: Content, offset: CGSize)

### Getting the shape’s characteristics

var offset: CGSize

var shape: Content

### Supporting types

var animatableData: OffsetShape&lt;Content>.AnimatableData

The data to animate.

## Relationships

### Conforms To

- Animatable

  Conforms when `Content` conforms to `InsettableShape`.

- Copyable
- InsettableShape

  Conforms when `Content` conforms to `InsettableShape`.

- Sendable
- Shape

  Conforms when `Content` conforms to `InsettableShape`.

- View

## See Also

### Transforming a shape

struct ScaledShape

A shape with a scale transform applied to it.

struct RotatedShape

A shape with a rotation transform applied to it.

struct TransformedShape

A shape with an affine transform applied to it.

