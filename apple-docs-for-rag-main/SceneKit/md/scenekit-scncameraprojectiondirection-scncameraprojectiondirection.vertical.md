

- SceneKit
- SCNCameraProjectionDirection
-  SCNCameraProjectionDirection.vertical 

Case

# SCNCameraProjectionDirection.vertical

The camera’s field of view or orthographic scale are measured vertically.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
case vertical
```

## Discussion

If a camera’s projectionDirection property has this value:

- The fieldOfView property measures the vertical viewing angle, and SceneKit automatically calculates the horizontal angle according to the aspect ratio of the view presenting the scene.

- Or, if the camera uses an orthographic projection, the orthographicScale property measures the vertical scale factor, and SceneKit automatically calculates the horizontal factor according to aspect ratio.

## See Also

### Projection Directions

case horizontal

The camera’s field of view or orthographic scale are measured horizontally.

