

- SpriteKit
- SKShapeNode
-  glowWidth 

Instance Property

# glowWidth

A glow that extends outward from the stroked line.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var glowWidth: CGFloat { get set }
```

**watchOS**

``` source
var glowWidth: CGFloat { get set }
```

## Mentioned in 

Getting Started with Shape Nodes

## Discussion

The default value is `0.0`, which means no glow is added. The glow color is determined by strokeColor.

## See Also

### Stroking a Shape

var lineWidth: CGFloat

The width used to stroke the path.

var strokeColor: UIColor

The color used to stroke the shape.

var strokeTexture: SKTexture?

The texture used to stroke the shape.

var lineCap: CGLineCap

The style used to render the endpoints of the stroked portion of the shape node.

var lineJoin: CGLineJoin

The junction type used when the stroked portion of the shape node is rendered.

var miterLimit: CGFloat

The miter limit to use when the line is stroked using a miter join style.

var isAntialiased: Bool

A Boolean value that determines whether the stroked path is smoothed when drawn.

