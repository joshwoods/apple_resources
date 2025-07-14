

- Core Foundation
-  CGRect 

Structure

# CGRect

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CGRect
```

## Topics

### Initializers

init()

init?(dictionaryRepresentation: CFDictionary)

init(origin: CGPoint, size: CGSize)

init(x: Double, y: Double, width: Double, height: Double)

init(x: Int, y: Int, width: Int, height: Int)

init(x: CGFloat, y: CGFloat, width: CGFloat, height: CGFloat)

### Instance Properties

var customPlaygroundQuickLook: PlaygroundQuickLook

A custom playground Quick Look for this instance.

Deprecated

var dictionaryRepresentation: CFDictionary

var height: CGFloat

var integral: CGRect

var isEmpty: Bool

var isInfinite: Bool

var isNull: Bool

var maxX: CGFloat

var maxY: CGFloat

var midX: CGFloat

var midY: CGFloat

var minX: CGFloat

var minY: CGFloat

var origin: CGPoint

var size: CGSize

var standardized: CGRect

var width: CGFloat

### Instance Methods

func applying(CGAffineTransform) -> CGRect

func clip()

Modifies the current graphics context clipping path by intersecting it with this rect. This permanently modifies the graphics state, so the current state should be saved beforehand and restored afterwards.

func contains(CGPoint) -> Bool

func contains(CGRect) -> Bool

func divided(atDistance: CGFloat, from: CGRectEdge) -> (slice: CGRect, remainder: CGRect)

func equalTo(CGRect) -> Bool

func fill(using: NSCompositingOperation)

Fills this rect in the current NSGraphicsContext in the context’s fill color. The compositing operation of the fill defaults to the context’s compositing operation, not necessarily using `.copy` like `NSRectFill()`.

func frame(withWidth: CGFloat, using: NSCompositingOperation)

Draws a frame around the inside of this rect in the current NSGraphicsContext in the context’s fill color The compositing operation of the fill defaults to the context’s compositing operation, not necessarily using `.copy` like `NSFrameRect()`.

func inset(by: UIEdgeInsets) -> CGRect

func insetBy(dx: CGFloat, dy: CGFloat) -> CGRect

func intersection(CGRect) -> CGRect

func intersects(CGRect) -> Bool

func offsetBy(dx: CGFloat, dy: CGFloat) -> CGRect

func union(CGRect) -> CGRect

### Type Properties

static var infinite: CGRect

static var null: CGRect

static var zero: CGRect

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

struct CGPoint

struct CGSize

A structure that contains width and height values.

struct CGVector

A structure that contains a two-dimensional vector.

