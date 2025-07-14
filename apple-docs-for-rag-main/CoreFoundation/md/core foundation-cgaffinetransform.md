

- Core Foundation
-  CGAffineTransform 

Structure

# CGAffineTransform

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CGAffineTransform
```

## Topics

### Initializers

init()

init(CGAffineTransformComponents)

init(CGFloat, CGFloat, CGFloat, CGFloat, CGFloat, CGFloat)

init(a: Double, b: Double, c: Double, d: Double, tx: Double, ty: Double)

init(rotationAngle: CGFloat)

init(scaleX: CGFloat, y: CGFloat)

init(translationX: CGFloat, y: CGFloat)

### Instance Properties

var a: Double

var b: Double

var c: Double

var d: Double

var isIdentity: Bool

var tx: Double

var ty: Double

### Instance Methods

func concatenating(CGAffineTransform) -> CGAffineTransform

func decomposed() -> CGAffineTransformComponents

func inverted() -> CGAffineTransform

func rotated(by: CGFloat) -> CGAffineTransform

func scaledBy(x: CGFloat, y: CGFloat) -> CGAffineTransform

func translatedBy(x: CGFloat, y: CGFloat) -> CGAffineTransform

### Type Properties

static var identity: CGAffineTransform

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Structures

struct CGAffineTransformComponents

struct CGFloat

The basic type for floating-point scalar values in Core Graphics and related frameworks.

struct CGPoint

struct CGRect

struct CGSize

A structure that contains width and height values.

struct CGVector

A structure that contains a two-dimensional vector.

