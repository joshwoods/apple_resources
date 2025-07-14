

- SceneKit
- SCNTorus
-  ringRadius 

Instance Property

# ringRadius

The major radius of the torus, defining a circle in the x- and z-axis dimensions. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var ringRadius: CGFloat { get set }
```

## Discussion

In the definition of a torus as a surface of revolution, the ring radius is the distance from the center of a circle (defined by the pipeRadius property) to the axis of revolution (the y-axis of the torus’s local coordinate space). Rotating the circle around the axis forms a pipe that follows a ring-shaped path.

The default ring radius is `0.5`. A ring radius of zero or less creates an empty geometry.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Adjusting a Torus’ Dimensions

var pipeRadius: CGFloat

The minor radius of the torus, defining the pipe that encircles the torus ring. Animatable.

