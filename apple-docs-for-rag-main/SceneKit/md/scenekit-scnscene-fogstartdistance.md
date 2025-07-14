

- SceneKit
- SCNScene
-  fogStartDistance 

Instance Property

# fogStartDistance

The distance from a point of view at which the scene’s contents begin to be obscured by fog. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var fogStartDistance: CGFloat { get set }
```

## Discussion

A fog effect causes scene contents to become less visible the farther they are from the pointOfView node currently used for rendering. At distances less than the value of the fogStartDistance property, scene contents are fully visible. At greater distances, SceneKit blends the rendered scene contents with a constant color (specified by the fogColor property). At distances greater than the fogEndDistance property, the scene contents fade away completely and only the fog color is visible. Use fog to add atmospheric effects to your app or game, or to improve rendering performance by hiding parts of the scene that are far away from the current point of view.

The default start distance is `0.0`.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Adding Fog to a Scene

var fogEndDistance: CGFloat

The distance from a point of view at which the scene’s contents are completely obscured by fog. Animatable.

var fogDensityExponent: CGFloat

The transition curve for the fog’s intensity between its start and end distances. Animatable.

var fogColor: Any

The color of the fog effect to be rendered with the scene. Animatable.

