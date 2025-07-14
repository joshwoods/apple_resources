

- SpriteKit
- SKView
-  showsFPS 

Instance Property

# showsFPS

A Boolean value that indicates whether the view displays a frame rate indicator.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@MainActor
var showsFPS: Bool { get set }
```

## Discussion

The frame rate is a good indicator of the performance of your scene. Avoid creating scenes that have widely varying frame rates.

## See Also

### Enabling Visual Statistics for Debugging

var showsNodeCount: Bool

A Boolean value that indicates whether the view displays an overlay that shows physics bodies that are visible in the scene.

var showsDrawCount: Bool

A Boolean value that indicates whether the view displays the number of drawing passes it needed to render the view.

var showsQuadCount: Bool

A Boolean value that indicates whether the view displays the number of rectangles used to render the scene.

var showsPhysics: Bool

A Boolean value that indicates whether the view displays physics-related debugging information.

var showsFields: Bool

A Boolean value that indicates whether the view displays information about physics fields in the scene.

