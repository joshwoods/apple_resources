

- SceneKit
- SCNText
-  extrusionDepth 

Instance Property

# extrusionDepth

The extent of the extruded text in the z-axis direction. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var extrusionDepth: CGFloat { get set }
```

## Discussion

The geometry is centered along the z-axis of its local coordinate space. For example, if its extrusion depth is is `1.0`, the geometry extends from `-0.5` to `0.5` along the z-axis.

An extrusion depth of `0.0` (the default) creates a flat, one-sided shape.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Managing the Text’s 3D Representation

var flatness: CGFloat

A number that determines the accuracy or smoothness of the text geometry.

var chamferRadius: CGFloat

The width or depth of each chamfered edge. Animatable.

var chamferProfile: UIBezierPath?

A path that determines the cross-sectional contour of each chamfered edge.

