

- SpriteKit
- SKShapeNode
-  lineCap 

Instance Property

# lineCap

The style used to render the endpoints of the stroked portion of the shape node.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var lineCap: CGLineCap { get set }
```

**watchOS**

``` source
var lineCap: CGLineCap { get set }
```

## Discussion

The default value is CGLineCap.butt. See CGLineCap.

## See Also

### Stroking a Shape

var lineWidth: CGFloat

The width used to stroke the path.

var strokeColor: UIColor

The color used to stroke the shape.

var strokeTexture: SKTexture?

The texture used to stroke the shape.

var glowWidth: CGFloat

A glow that extends outward from the stroked line.

var lineJoin: CGLineJoin

The junction type used when the stroked portion of the shape node is rendered.

var miterLimit: CGFloat

The miter limit to use when the line is stroked using a miter join style.

var isAntialiased: Bool

A Boolean value that determines whether the stroked path is smoothed when drawn.

