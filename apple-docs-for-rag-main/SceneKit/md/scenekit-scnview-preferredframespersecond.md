

- SceneKit
- SCNView
-  preferredFramesPerSecond 

Instance Property

# preferredFramesPerSecond

The animation frame rate that the view uses to render its scene.

iOSiPadOSMac Catalyst 13.1+macOS 10.12+tvOSvisionOS

``` source
@MainActor
var preferredFramesPerSecond: Int { get set }
```

## Discussion

SceneKit chooses an actual frame rate that is as close as possible to your preferred frame rate based on the capabilities of the screen the view is displayed on. The actual frame rate is usually a factor of the maximum refresh rate of the screen to provide a consistent frame rate. For example, if the maximum refresh rate of the screen is `60` frames per second, that is also the highest frame rate the view sets as the actual frame rate. However, if you ask for a lower frame rate, SceneKit might choose `30`, `20`, `15` or some other factor to be the actual frame rate. For this reason, you want to choose a frame rate that your app can consistently maintain.

The default value is `60` frames per second.

## See Also

### Configuring a View

var backgroundColor: NSColor

The background color of the view.

var rendersContinuously: Bool

A Boolean value that determines whether the view always renders at its preferred frame rate or only when its visible content changes.

var antialiasingMode: SCNAntialiasingMode

The antialiasing mode used for rendering the view’s scene.

enum SCNAntialiasingMode

Modes for antialiased rendering of the view’s scene, used by the SCNView property.

