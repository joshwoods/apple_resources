

- SpriteKit
- SKView
-  showsPhysics 

Instance Property

# showsPhysics

A Boolean value that indicates whether the view displays physics-related debugging information.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var showsPhysics: Bool { get set }
```

## Discussion

When this debugging option is enabled, each time a frame is rendered, an overlay image is drawn on top of your scene that shows the positions and shapes of any physics bodies visible in the scene.

## See Also

### Enabling Visual Statistics for Debugging

var showsFPS: Bool

A Boolean value that indicates whether the view displays a frame rate indicator.

var showsNodeCount: Bool

A Boolean value that indicates whether the view displays an overlay that shows physics bodies that are visible in the scene.

var showsDrawCount: Bool

A Boolean value that indicates whether the view displays the number of drawing passes it needed to render the view.

var showsQuadCount: Bool

A Boolean value that indicates whether the view displays the number of rectangles used to render the scene.

var showsFields: Bool

A Boolean value that indicates whether the view displays information about physics fields in the scene.

