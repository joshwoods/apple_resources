

- SpriteKit
- SKView
-  showsNodeCount 

Instance Property

# showsNodeCount

A Boolean value that indicates whether the view displays an overlay that shows physics bodies that are visible in the scene.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@MainActor
var showsNodeCount: Bool { get set }
```

## Mentioned in 

Maximizing Node Drawing Performance

## Discussion

When you enable this option, it shows the number of nodes currently in the scene’s node tree.

Note

TheshouldCullNonVisibleNodes property affects how many nodes in the node tree are included in SpriteKit’s render pass but it doesn’t affect the showsNodeCount statistic.

You may achieve additional performance gain by actually removing nodes from the node tree manually which are off screen. For example, in the case of shouldCullNonVisibleNodes, there would be less nodes for SpriteKit to test every frame whether they’re on screen.

## See Also

### Enabling Visual Statistics for Debugging

var showsFPS: Bool

A Boolean value that indicates whether the view displays a frame rate indicator.

var showsDrawCount: Bool

A Boolean value that indicates whether the view displays the number of drawing passes it needed to render the view.

var showsQuadCount: Bool

A Boolean value that indicates whether the view displays the number of rectangles used to render the scene.

var showsPhysics: Bool

A Boolean value that indicates whether the view displays physics-related debugging information.

var showsFields: Bool

A Boolean value that indicates whether the view displays information about physics fields in the scene.

