

- SwiftUI
-  TransformedShape 

Structure

# TransformedShape

A shape with an affine transform applied to it.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct TransformedShape where Content : Shape
```

## Topics

### Creating a transformed shape

init(shape: Content, transform: CGAffineTransform)

### Getting the shape’s characteristics

var shape: Content

var transform: CGAffineTransform

## Relationships

### Conforms To

- Animatable
- Sendable
- Shape
- View

## See Also

### Transforming a shape

struct ScaledShape

A shape with a scale transform applied to it.

struct RotatedShape

A shape with a rotation transform applied to it.

struct OffsetShape

A shape with a translation offset transform applied to it.

