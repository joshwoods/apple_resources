

- Spatial
- Rotation3D
- Rotation3D.SlerpPath
-  Rotation3D.SlerpPath.automatic 

Case

# Rotation3D.SlerpPath.automatic

Spherical linear interpolation along the automatically selected arc between two rotations.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
case automatic
```

## Discussion

For angular separations that are less than or equal to 180°, the spherical linear interpolation along the shortest arc between two rotations, otherwise along the longest arc.

## See Also

### Enumeration Cases

case shortest

Spherical linear interpolation along the shortest arc between two rotations.

case longest

Spherical linear interpolation along the longest arc between two rotations.

