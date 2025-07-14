

- SpriteKit
- SKShapeNode
-  fillTexture 

Instance Property

# fillTexture

The texture used to fill the shape.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var fillTexture: SKTexture? { get set }
```

**watchOS**

``` source
var fillTexture: SKTexture? { get set }
```

## Mentioned in 

Controlling Shape Drawing with Shaders

## Discussion

The default value is `nil`. If a fill texture is specified, the shape node is rendered using that texture blended with the fillColor.

Important

The default fill color of a SKShapeNode is `SKColor.clear`. Since the fill texture is blended with the fill color, fillColor needs to be set to a non-clear color for it to display. For example, to display the texture without any color blend effects, set fillColor to `SKColor.white`.

## See Also

### Filling a Shape

var fillColor: UIColor

The color used to fill the shape.

