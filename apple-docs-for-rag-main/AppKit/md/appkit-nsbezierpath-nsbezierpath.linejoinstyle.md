

- AppKit
- NSBezierPath
-  NSBezierPath.LineJoinStyle 

Enumeration

# NSBezierPath.LineJoinStyle

Constants that specify the shape of the joins between connected segments of a stroked path.

macOS

``` source
enum LineJoinStyle
```

## Topics

### Constants

case miter

Specifies a miter line shape of the joints between connected segments of a stroked path.

case round

Specifies a round line shape of the joints between connected segments of a stroked path.

case bevel

Specifies a bevel line shape of the joints between connected segments of a stroked path.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum ElementType

Constants that specify basic path element commands.

enum LineCapStyle

Constants that specify the shape of endpoints for an open path when it is stroked.

enum WindingRule

Constants that specify the winding rule a Bézier path uses.

