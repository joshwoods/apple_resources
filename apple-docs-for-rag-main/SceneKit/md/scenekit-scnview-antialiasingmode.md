

- SceneKit
- SCNView
-  antialiasingMode 

Instance Property

# antialiasingMode

The antialiasing mode used for rendering the view’s scene.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOS

``` source
@MainActor
var antialiasingMode: SCNAntialiasingMode { get set }
```

## Discussion

SceneKit can provide antialiasing, which smooths edges in a rendered scene, using a technique called *multisampling*. Multisampling renders each pixel multiple times and combines the results, creating a higher quality image at a performance cost proportional to the number of samples it uses.

For available values, see SCNView. In macOS, the default mode is SCNAntialiasingMode.multisampling4X. In iOS, the default mode is SCNAntialiasingMode.none.

## See Also

### Configuring a View

var backgroundColor: NSColor

The background color of the view.

var preferredFramesPerSecond: Int

The animation frame rate that the view uses to render its scene.

var rendersContinuously: Bool

A Boolean value that determines whether the view always renders at its preferred frame rate or only when its visible content changes.

enum SCNAntialiasingMode

Modes for antialiased rendering of the view’s scene, used by the SCNView property.

