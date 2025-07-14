

- SceneKit
- SCNShape
-  extrusionDepth 

Instance Property

# extrusionDepth

The thickness of the extruded shape along the z-axis. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
var extrusionDepth: CGFloat { get set }
```

## Discussion

The extruded shape is centered at the zero point of its z-axis. For example, an extrusion depth of `1.0` creates a shape that extends from `-0.5` to `0.5` along the z-axis. An extrusion depth of zero creates a flat, one-sided shape.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Modifying a Shape

var path: UIBezierPath?

The two-dimensional path forming the basis of the shape.

