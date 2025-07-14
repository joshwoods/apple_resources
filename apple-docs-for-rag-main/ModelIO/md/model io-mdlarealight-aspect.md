

- Model I/O
- MDLAreaLight
-  aspect 

Instance Property

# aspect

The aspect ratio of the light’s shape.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var aspect: Float { get set }
```

## Discussion

If the light’s type is MDLLightType.discArea, MDLLightType.rectangularArea, or MDLLightType.superElliptical, this property determines the lengths of the shape’s major and minor axes (longer and shorter dimensions) relative to the areaRadius property’s value.

## See Also

### Managing a Light’s Shape

var areaRadius: Float

The radius, in units of local coordinate space, of the area from which light emanates.

var superEllipticPower: vector_float2

A vector that controls the roundness of a superelliptical light in the x- and y-axis directions.

