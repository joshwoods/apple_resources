

- SpriteKit
- SKView
-  ignoresSiblingOrder 

Instance Property

# ignoresSiblingOrder

A Boolean value that indicates whether parent-child and sibling relationships affect the rendering order of nodes in the scene.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@MainActor
var ignoresSiblingOrder: Bool { get set }
```

## Mentioned in 

About Node Drawing Order

Maximizing Node Drawing Performance

## Discussion

The default value is false, which means that when multiple nodes share the same z position, those nodes are sorted and rendered in a deterministic order. Parents are rendered before their children, and siblings are rendered in array order. When this property is set to true, the position of the nodes in the tree is ignored when determining the rendering order. The rendering order of nodes at the same z position is arbitrary and may change every time a new frame is rendered. When sibling and parent order is ignored, SpriteKit applies additional optimizations to improve rendering performance. If you need nodes to be rendered in a specific and deterministic order, you must set the z position of those nodes.

## See Also

### Configuring Performance Related Toggles

var shouldCullNonVisibleNodes: Bool

A Boolean value that indicates whether the view automatically culls non-visible nodes from the rendering tree.

var allowsTransparency: Bool

A Boolean property that indicates whether the view is rendered using transparency.

var isAsynchronous: Bool

A Boolean value that indicates whether the content is rendered asynchronously.

