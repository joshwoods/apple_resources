

- SpriteKit
- SKNode
-  alpha 

Instance Property

# alpha

The transparency value applied to the node’s contents.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var alpha: CGFloat { get set }
```

**watchOS**

``` source
var alpha: CGFloat { get set }
```

## Mentioned in 

Controlling User Interaction on Nodes

About Node Property Propagation

Getting Started with Nodes

## Discussion

The default value is `1.0`.

The SKNode class does not perform drawing, but many of its subclasses do. When a node or any of its descendants are drawn, the alpha component of each pixel is multiplied by the node’s alpha property and then clamped to the range `0.0`-`1.0`. This modified alpha value is used to blend the pixel into the framebuffer. Subclasses that render content define properties that determine the blending operations used in conjunction with the alpha value to blend pixels into the parent’s framebuffer.

## See Also

### Altering Node Visibility

var isHidden: Bool

A Boolean value that determines whether a node and its descendants are rendered.

