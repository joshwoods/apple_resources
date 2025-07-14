

- SpriteKit
- SKShapeNode
-  miterLimit 

Instance Property

# miterLimit

The miter limit to use when the line is stroked using a miter join style.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var miterLimit: CGFloat { get set }
```

**watchOS**

``` source
var miterLimit: CGFloat { get set }
```

## Discussion

If the line join style is set to CGLineJoin.miter, SpriteKit uses the miter limit to determine whether the lines should be joined with a bevel instead of a miter. SpriteKit divides the length of the miter by the line width. If the result is greater than the miter limit, SpriteKit converts the style to a bevel.

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

var isAntialiased: Bool

A Boolean value that determines whether the stroked path is smoothed when drawn.

