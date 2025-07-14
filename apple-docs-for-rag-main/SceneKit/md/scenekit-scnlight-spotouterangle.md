

- SceneKit
- SCNLight
-  spotOuterAngle 

Instance Property

# spotOuterAngle

The angle, in degrees, of the area partially lit by a spotlight. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var spotOuterAngle: CGFloat { get set }
```

## Discussion

You define the cone-shaped illuminated area of a spotlight with a position and direction (from the node containing the light) and with an angle specifying the cone’s width. Additionally, the illuminated area can smoothly transition from full illumination to no illumination. This property determines the width of the transition area.

The default value is `45.0`.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Managing Spotlight Extent

var spotInnerAngle: CGFloat

The angle, in degrees, of the area fully lit by a spotlight. Animatable.

var gobo: SCNMaterialProperty?

An image or other visual content affecting the shape and color of a light’s illuminated area.

