

- RealityKit
- OrthographicCameraComponent
-  near 

Instance Property

# near

The minimum distance in meters from the camera that the camera can see.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var near: Float
```

## Discussion

The value defaults to `1.0` centimeter. Use a value greater than `0.0` and less than the value of far. The renderer clips any surface closer than the `near` point.

## See Also

### Setting focal points

var far: Float

The maximum distance in meters from the camera that the camera can see.

