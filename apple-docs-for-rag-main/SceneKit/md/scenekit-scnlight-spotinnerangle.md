

- SceneKit
- SCNLight
-  spotInnerAngle 

Instance Property

# spotInnerAngle

The angle, in degrees, of the area fully lit by a spotlight. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var spotInnerAngle: CGFloat { get set }
```

## Discussion

You define the cone-shaped illuminated area of a spotlight with a position and direction (from the node containing the light) and an angle specifying the cone’s width. Additionally, the illuminated area can smoothly transition from full illumination to no illumination. This property determines the width of the fully illuminated area.

The default value is `0.0`, specifying that only the center of the area illuminated by the spotlight is lit at full intensity.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Managing Spotlight Extent

var spotOuterAngle: CGFloat

The angle, in degrees, of the area partially lit by a spotlight. Animatable.

var gobo: SCNMaterialProperty?

An image or other visual content affecting the shape and color of a light’s illuminated area.

