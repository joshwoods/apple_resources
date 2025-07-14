

- Model I/O
- MDLAreaLight
-  areaRadius 

Instance Property

# areaRadius

The radius, in units of local coordinate space, of the area from which light emanates.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var areaRadius: Float { get set }
```

## Discussion

The effect of radius on a light’s shape depends on the value of its inherited lightType property:

- MDLLightType.linear: The light is shaped like a line segment, centered on the origin of its local coordinate space and extending along the x-axis with a total length of twice the areaRadius value.

- MDLLightType.discArea: The light is shaped like a circle or ellipse in the xy-plane of its local coordinate space. If the aspect value is `1.0`, the areaRadius value is the circle’s radius. If the aspect value is less than one, the areaRadius value is the major radius of the ellipse, and the minor radius is equal to the areaRadius value times the aspect value.

- MDLLightType.rectangularArea: The light is shaped like a rectangle in the xy-plane of its local coordinate space. If the aspect value is `1.0`, the light is a square and areaRadius value is half the square’s width or length. If the aspect value is less than one, the areaRadius value is half the rectangle’s longer dimension, and the shorter dimension is the areaRadius value, times the aspect value, times two.

- MDLLightType.superElliptical: The light is shaped like a superellipse—a two-dimensional figure in the xy-plane of its local coordinate space that can vary between shapes such as stars, diamonds, circles, and squares with rounded corners. The superEllipticPower property determines the general shape of the light, and the aspect property controls the ratio of the longer and shorter dimensions of the shape.

## See Also

### Managing a Light’s Shape

var aspect: Float

The aspect ratio of the light’s shape.

var superEllipticPower: vector_float2

A vector that controls the roundness of a superelliptical light in the x- and y-axis directions.

