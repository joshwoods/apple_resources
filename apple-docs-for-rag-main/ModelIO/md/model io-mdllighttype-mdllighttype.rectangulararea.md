

- Model I/O
- MDLLightType
-  MDLLightType.rectangularArea 

Case

# MDLLightType.rectangularArea

The light source illuminates a scene in all directions from an area in the shape of a rectangle.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
case rectangularArea
```

## Discussion

This light type is exclusive to the MDLAreaLight class.

## See Also

### Constants

case unknown

The type of the light is unknown or has not been initialized.

case ambient

The light source should illuminate a scene evenly regardless of position or direction.

case directional

The light source illuminates a scene from a uniform direction regardless of its position.

case spot

The light source illuminates a scene from a specific position and direction.

case point

The light source illuminates a scene in all directions from a specific position.

case linear

The light source illuminates a scene in all directions from an area in the shape of a line.

case discArea

The light source illuminates a scene in all directions from an area in the shape of a disc.

case superElliptical

The light source illuminates a scene in all directions from an area in the shape of a superellipse.

case photometric

The illumination from the light is determined by a photometric profile.

case probe

The illumination from the light is determined by texture images representing a sample of a scene at a specific point.

case environment

The illumination from the light is determined by texture images representing a sample of the surrounding environment for a scene.

