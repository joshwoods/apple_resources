

- SceneKit
- SCNScene
-  fogColor 

Instance Property

# fogColor

The color of the fog effect to be rendered with the scene. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var fogColor: Any { get set }
```

## Discussion

This property’s value can be an NSColor object (in macOS), a UIColor object (in iOS), or a CGColor object. The default fog color is white.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Adding Fog to a Scene

var fogStartDistance: CGFloat

The distance from a point of view at which the scene’s contents begin to be obscured by fog. Animatable.

var fogEndDistance: CGFloat

The distance from a point of view at which the scene’s contents are completely obscured by fog. Animatable.

var fogDensityExponent: CGFloat

The transition curve for the fog’s intensity between its start and end distances. Animatable.

