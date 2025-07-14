

- SpriteKit
- SKNode
-  zPosition 

Instance Property

# zPosition

The height of the node relative to its parent.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
var zPosition: CGFloat { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var zPosition: CGFloat { get set }
```

## Mentioned in 

Maximizing Node Drawing Performance

About Node Drawing Order

About Node Property Propagation

Getting Started with Nodes

Controlling User Interaction on Nodes

## Discussion

The default value is `0.0`. The positive z axis is projected toward the viewer so that nodes with larger z-position values are closer to the viewer. When a node tree is rendered, the height of each node (in absolute coordinates) is calculated and then all nodes in the tree are rendered from smallest z-position value to largest z-position value. If multiple nodes share the same z-position, those nodes are sorted so that parent nodes are drawn before their children, and siblings are rendered in the order that they appear in their parent’s children array. Hit-testing is processed in the opposite order.

The SKView class’s ignoresSiblingOrder property controls whether node sorting is enabled for nodes at the same z-position.

Important

Descendants of an effect node or a crop node are not rendered with other nodes in the same tree. An effect node (SKEffectNode) renders its children into a private framebuffer as a separate node tree, then the composited image is rendered into the tree that contains the effect node. A crop node (SKCropNode) works similarly; it renders the mask separately, then uses the mask to render its actual descendants into the tree that contains the crop node.

### Using a Node’s Depth to Add Effects

SpriteKit uses the zPosition value only to determine the hit testing and drawing order. You can also the z position to implement your own game effects. For example, you might use the height of a node to determine how it is rendered or how it moves onscreen. In this way, you can simulate fog or parallax effects. SpriteKit does not create these effects for you. Usually, you implement them by processing the scene immediately before it is rendered.

## See Also

### Configuring Draw Order

About Node Drawing Order

Understand how SpriteKit layers your scene’s nodes from top to bottom.

