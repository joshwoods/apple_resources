

- SceneKit
- SCNText
-  flatness 

Instance Property

# flatness

A number that determines the accuracy or smoothness of the text geometry.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
var flatness: CGFloat { get set }
```

## Discussion

SceneKit uses line segments to approximate the curved shapes of text characters when converting text into a three-dimensional geometry. (These segments become side polygons when SceneKit extrudes the text.) Higher flatness values result in fewer segments, reducing the smoothness of curves and improving rendering performance. Lower values result in more segments, increasing the smoothness of curves at a cost to rendering performance.

The default value of this property is `0.6`, specifying that the line segments may not deviate from the curve by more than 0.6 points.

## See Also

### Managing the Text’s 3D Representation

var extrusionDepth: CGFloat

The extent of the extruded text in the z-axis direction. Animatable.

var chamferRadius: CGFloat

The width or depth of each chamfered edge. Animatable.

var chamferProfile: UIBezierPath?

A path that determines the cross-sectional contour of each chamfered edge.

