

- Model I/O
- MDLPhysicallyPlausibleLight
-  innerConeAngle 

Instance Property

# innerConeAngle

The radial angle, in degrees, of the area fully illuminated by the light.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var innerConeAngle: Float { get set }
```

## Discussion

This property measures the angle from the light axis (the direction in which the light points; the negative z-axis of its local coordinate space) to the edge of the light’s effect. For example, a cone angle of 22.5 degrees (the default) creates a broad spot light. (The light’s lightType value is MDLLightType.spot.) An angle of 90 degrees divides space evenly, illuminating in all directions in front of the light and none behind, and an angle of 180 degrees illuminates in all directions (creating a light whose type is MDLLightType.point).

## See Also

### Managing Light Geometry

var outerConeAngle: Float

The radial angle, in degrees, at which the illumination from a spotlight becomes zero.

