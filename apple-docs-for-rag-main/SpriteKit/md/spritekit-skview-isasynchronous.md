

- SpriteKit
- SKView
-  isAsynchronous 

Instance Property

# isAsynchronous

A Boolean value that indicates whether the content is rendered asynchronously.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@MainActor
var isAsynchronous: Bool { get set }
```

## Discussion

The default value is true. If the value is false, the contents of this view are synchronized with Core Animation updates.

## See Also

### Configuring Performance Related Toggles

var ignoresSiblingOrder: Bool

A Boolean value that indicates whether parent-child and sibling relationships affect the rendering order of nodes in the scene.

var shouldCullNonVisibleNodes: Bool

A Boolean value that indicates whether the view automatically culls non-visible nodes from the rendering tree.

var allowsTransparency: Bool

A Boolean property that indicates whether the view is rendered using transparency.

