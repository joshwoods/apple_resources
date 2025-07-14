

- SceneKit
- SCNView
-  rendersContinuously 

Instance Property

# rendersContinuously

A Boolean value that determines whether the view always renders at its preferred frame rate or only when its visible content changes.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@MainActor
var rendersContinuously: Bool { get set }
```

## Discussion

When this value is false (the default), the view redraws its contents only when something in its scene graph change or animates. Use this option to maximize energy efficiency.

If you change this value to true, the view redraws itself continually, at the rate specified by the preferredFramesPerSecond property, regardless of whether content is changing or animating.

## See Also

### Configuring a View

var backgroundColor: NSColor

The background color of the view.

var preferredFramesPerSecond: Int

The animation frame rate that the view uses to render its scene.

var antialiasingMode: SCNAntialiasingMode

The antialiasing mode used for rendering the view’s scene.

enum SCNAntialiasingMode

Modes for antialiased rendering of the view’s scene, used by the SCNView property.

