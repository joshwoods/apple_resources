

- SpriteKit
- SKShapeNode
-  strokeTexture 

Instance Property

# strokeTexture

The texture used to stroke the shape.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var strokeTexture: SKTexture? { get set }
```

**watchOS**

``` source
var strokeTexture: SKTexture? { get set }
```

## Discussion

The default value is `nil`. If a stroke texture is specified, the strokeColor property is ignored and the stroked portion of the shape node is rendered using the texture instead.

## See Also

### Stroking a Shape

var lineWidth: CGFloat

The width used to stroke the path.

var strokeColor: UIColor

The color used to stroke the shape.

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

