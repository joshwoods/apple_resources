

- SpriteKit
- SKView
-  showsQuadCount 

Instance Property

# showsQuadCount

A Boolean value that indicates whether the view displays the number of rectangles used to render the scene.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var showsQuadCount: Bool { get set }
```

## Discussion

SpriteKit converts the node tree into one or more rendering passes. Each rendering pass is rendered using a series of textured rectangles (quads). The showsQuadCount property allows you to see the total number of quads that were used to render the scene’s contents. Use this as another piece of data when you profile your game’s performance. In most cases, fewer quads is better.

## See Also

### Enabling Visual Statistics for Debugging

var showsFPS: Bool

A Boolean value that indicates whether the view displays a frame rate indicator.

var showsNodeCount: Bool

A Boolean value that indicates whether the view displays an overlay that shows physics bodies that are visible in the scene.

var showsDrawCount: Bool

A Boolean value that indicates whether the view displays the number of drawing passes it needed to render the view.

var showsPhysics: Bool

A Boolean value that indicates whether the view displays physics-related debugging information.

var showsFields: Bool

A Boolean value that indicates whether the view displays information about physics fields in the scene.

