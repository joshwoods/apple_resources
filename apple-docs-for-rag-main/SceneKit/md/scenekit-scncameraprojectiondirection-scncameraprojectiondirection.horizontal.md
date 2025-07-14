

- SceneKit
- SCNCameraProjectionDirection
-  SCNCameraProjectionDirection.horizontal 

Case

# SCNCameraProjectionDirection.horizontal

The camera’s field of view or orthographic scale are measured horizontally.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
case horizontal
```

## Discussion

If a camera’s projectionDirection property has this value:

- The fieldOfView property measures the horizontal viewing angle, and SceneKit automatically calculates the vertical angle according to the aspect ratio of the view presenting the scene.

- Or, if the camera uses an orthographic projection, the orthographicScale property measures the horizontal scale factor, and SceneKit automatically calculates the vertical factor according to aspect ratio.

## See Also

### Projection Directions

case vertical

The camera’s field of view or orthographic scale are measured vertically.

