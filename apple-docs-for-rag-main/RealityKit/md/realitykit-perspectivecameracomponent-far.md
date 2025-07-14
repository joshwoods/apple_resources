

- RealityKit
- PerspectiveCameraComponent
-  far 

Instance Property

# far

The maximum distance in meters from the camera that the camera can see.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
var far: Float
```

## Discussion

The value defaults to `infinity`. Use a value greater than the value of near. The renderer clips any surface beyond the `far` point.

## See Also

### Setting focal points

var near: Float

The minimum distance in meters from the camera that the camera can see.

