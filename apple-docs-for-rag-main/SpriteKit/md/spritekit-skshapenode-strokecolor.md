

- SpriteKit
- SKShapeNode
-  strokeColor 

Instance Property

# strokeColor

The color used to stroke the shape.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
var strokeColor: UIColor { get set }
```

**watchOS**

``` source
var strokeColor: UIColor { get set }
```

**macOS**

``` source
@MainActor
var strokeColor: NSColor { get set }
```

## Mentioned in 

Getting Started with Shape Nodes

## Discussion

The default stroke color is `[SKColor whiteColor]`. If you do not want to stroke the shape, use `[SKColor clearColor].`

## See Also

### Stroking a Shape

var lineWidth: CGFloat

The width used to stroke the path.

var strokeTexture: SKTexture?

The texture used to stroke the shape.

var glowWidth: CGFloat

A glow that extends outward from the stroked line.

var lineCap: CGLineCap

The style used to render the endpoints of the stroked portion of the shape node.

var lineJoin: CGLineJoin

The junction type used when the stroked portion of the shape node is rendered.

var miterLimit: CGFloat

The miter limit to use when the line is stroked using a miter join style.

var isAntialiased: Bool

A Boolean value that determines whether the stroked path is smoothed when drawn.

