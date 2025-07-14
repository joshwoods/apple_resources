

- Compositor Services
-  AxisDirectionConvention 

Enumeration

# AxisDirectionConvention

Constants that indicate the axis and direction to use for a perspective projection matrix.

visionOS 2.0+

``` source
enum AxisDirectionConvention
```

## Topics

### Getting the axis directions

case rightUpBack

The convention that uses a counterclockwise winding order and positions the leading pixel at the top-left corner of the view.

case rightUpForward

The convention that uses a clockwise winding order and positions the leading pixel at the top-left corner of the view.

case rightDownBack

The convention that uses a counterclockwise winding order and positions the leading pixel at the bottom-left corner of the view.

case rightDownForward

The convention that uses a clockwise winding order and positions the leading pixel at the bottom-left corner of the view.

### Initializers

init?(rawValue: UInt8)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

