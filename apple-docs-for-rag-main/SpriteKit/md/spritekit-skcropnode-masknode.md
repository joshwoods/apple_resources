

- SpriteKit
- SKCropNode
-  maskNode 

Instance Property

# maskNode

The node used to determine the crop node’s mask.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
var maskNode: SKNode? { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var maskNode: SKNode? { get set }
```

## Mentioned in 

Cropping Nodes

## Discussion

The node supplied to the crop node must not be a child of another node; however, it may have children of its own.

When the crop node’s contents are rendered, the crop node first draws its mask into a private buffer. Then, it renders its children. When rendering its children, each pixel is verified against the corresponding pixel in the mask. If the pixel in the mask has an alpha value of less than 0.05, the image pixel is masked out. Any pixel not rendered by the mask node is automatically masked out.

The default value of this property is `nil`, which indicates that the child nodes should not be cropped.

