

- ARKit
- ARPlaneAnchor
- ARPlaneAnchor.Alignment
-  ARPlaneAnchor.Alignment.horizontal 

Case

# ARPlaneAnchor.Alignment.horizontal

The plane is perpendicular to gravity.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
case horizontal
```

## Discussion

The transform property for a horizontal plane anchor includes no rotation about the x- or z-axis. Thus, using this anchor’s transform to place a 3D model asset in your scene results in the model appearing “right side up”.

## See Also

### Alignment Values

case vertical

The plane is parallel to gravity.

