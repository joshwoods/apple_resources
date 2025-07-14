

- Core Foundation
-  CGVector 

Structure

# CGVector

A structure that contains a two-dimensional vector.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CGVector
```

## Topics

### Special Values

static var zero: CGVector { get }

init()

Creates a vector whose components are both zero.

### Geometric Properties

var dx: Double

The x component of the vector.

var dy: Double

The y component of the vector.

### Initializers

init(dx: Double, dy: Double)

init(dx: Double, dy: Double)

init(dx: Int, dy: Int)

### Type Properties

static var zero: CGVector

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- CustomDebugStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Structures

struct CGAffineTransform

struct CGAffineTransformComponents

struct CGFloat

The basic type for floating-point scalar values in Core Graphics and related frameworks.

struct CGPoint

struct CGRect

struct CGSize

A structure that contains width and height values.

