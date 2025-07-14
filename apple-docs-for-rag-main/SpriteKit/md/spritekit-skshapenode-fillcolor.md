

- SpriteKit
- SKShapeNode
-  fillColor 

Instance Property

# fillColor

The color used to fill the shape.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**macOS**

``` source
@MainActor
var fillColor: NSColor { get set }
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
var fillColor: UIColor { get set }
```

**watchOS**

``` source
var fillColor: UIColor { get set }
```

## Mentioned in 

Controlling Shape Drawing with Shaders

Getting Started with Shape Nodes

## Discussion

The default fill color is `[SKColor clearColor]`, which means the shape is not filled.

## See Also

### Filling a Shape

var fillTexture: SKTexture?

The texture used to fill the shape.

