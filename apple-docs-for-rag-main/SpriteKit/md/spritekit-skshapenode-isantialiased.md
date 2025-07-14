

- SpriteKit
- SKShapeNode
-  isAntialiased 

Instance Property

# isAntialiased

A Boolean value that determines whether the stroked path is smoothed when drawn.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var isAntialiased: Bool { get set }
```

**watchOS**

``` source
var isAntialiased: Bool { get set }
```

## Discussion

The default value is true.

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

var lineCap: CGLineCap

The style used to render the endpoints of the stroked portion of the shape node.

var lineJoin: CGLineJoin

The junction type used when the stroked portion of the shape node is rendered.

var miterLimit: CGFloat

The miter limit to use when the line is stroked using a miter join style.

