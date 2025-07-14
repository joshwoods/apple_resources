

- SpriteKit
- SKShapeNode
-  lineWidth 

Instance Property

# lineWidth

The width used to stroke the path.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
var lineWidth: CGFloat { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var lineWidth: CGFloat { get set }
```

## Mentioned in 

Getting Started with Shape Nodes

## Discussion

A line width larger than `2.0` may cause rendering artifacts in the final rendered image. The default value is `1.0`.

## See Also

### Stroking a Shape

var strokeColor: UIColor

The color used to stroke the shape.

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

