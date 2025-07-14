

- SceneKit
- SCNLight
-  gobo 

Instance Property

# gobo

An image or other visual content affecting the shape and color of a light’s illuminated area.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
var gobo: SCNMaterialProperty? { get }
```

## Discussion

In photographic and stage lighting terminology, a gobo (also known as a *flag* or *cookie*) is a stencil, gel, or other object placed just in front of a light source, shaping or coloring the beam of light.

You alter the appearance of a spotlight by changing the contents property of the object permanently assigned to this property. As with other material properties, you can use a color or image, or a Core Animation layer containing animated content, as a lighting gobo.

This property applies only to lights whose type property is spot.

## See Also

### Managing Spotlight Extent

var spotInnerAngle: CGFloat

The angle, in degrees, of the area fully lit by a spotlight. Animatable.

var spotOuterAngle: CGFloat

The angle, in degrees, of the area partially lit by a spotlight. Animatable.

