

- Model I/O
- MDLPhysicallyPlausibleLight
-  outerConeAngle 

Instance Property

# outerConeAngle

The radial angle, in degrees, at which the illumination from a spotlight becomes zero.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var outerConeAngle: Float { get set }
```

## Discussion

This property measures the angle from the light axis (the direction in which the light points; the negative z-axis of its local coordinate space) to the edge of the region affected by the light. Between this value and that of the innerConeAngle property, the light’s intensity varies linearly.

The default value is 22.5 degrees, matching the default inner cone angle and thus creating a hard-edged spotlight. Set the outer cone angle greater than the inner cone angle to create a soft-edged spotlight.

## See Also

### Managing Light Geometry

var innerConeAngle: Float

The radial angle, in degrees, of the area fully illuminated by the light.

