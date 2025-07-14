

- SceneKit
- SCNView
-  backgroundColor 

Instance Property

# backgroundColor

The background color of the view.

macOS

``` source
@NSCopying @MainActor
var backgroundColor: NSColor { get set }
```

## Discussion

SceneKit displays this color behind the contents of the rendered scene. If the scene contents fill the view or if the scene provides its own background using the background property, the view’s background color may not be visible.

This property’s value must be a color that can be represented using RGBA components.

## See Also

### Configuring a View

var preferredFramesPerSecond: Int

The animation frame rate that the view uses to render its scene.

var rendersContinuously: Bool

A Boolean value that determines whether the view always renders at its preferred frame rate or only when its visible content changes.

var antialiasingMode: SCNAntialiasingMode

The antialiasing mode used for rendering the view’s scene.

enum SCNAntialiasingMode

Modes for antialiased rendering of the view’s scene, used by the SCNView property.

