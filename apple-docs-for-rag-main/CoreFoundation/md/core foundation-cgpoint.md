

- Core Foundation
-  CGPoint 

Structure

# CGPoint

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CGPoint
```

## Topics

### Initializers

init()

init?(dictionaryRepresentation: CFDictionary)

init(x: Double, y: Double)

init(x: Double, y: Double)

init(x: Int, y: Int)

### Instance Properties

var customPlaygroundQuickLook: PlaygroundQuickLook

A custom playground Quick Look for this instance.

Deprecated

var dictionaryRepresentation: CFDictionary

var x: Double

var y: Double

### Instance Methods

func applying(CGAffineTransform) -> CGPoint

func applying(ProjectionTransform) -> CGPoint

func equalTo(CGPoint) -> Bool

### Type Properties

static var zero: CGPoint

## Relationships

### Conforms To

- Animatable
- BitwiseCopyable
- Copyable
- CustomDebugStringConvertible
- CustomReflectable
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

struct CGRect

struct CGSize

A structure that contains width and height values.

struct CGVector

A structure that contains a two-dimensional vector.

