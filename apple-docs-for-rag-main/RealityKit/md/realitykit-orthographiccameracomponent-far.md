

- RealityKit
- OrthographicCameraComponent
-  far 

Instance Property

# far

The maximum distance in meters from the camera that the camera can see.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var far: Float
```

## Discussion

The value defaults to `1000.0`. Use a value greater than the value of near. The renderer clips any surface beyond the `far` point.

## See Also

### Setting focal points

var near: Float

The minimum distance in meters from the camera that the camera can see.

