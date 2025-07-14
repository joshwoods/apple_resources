

- Vision
- RectangleObservation
-  init(topLeft:topRight:bottomRight:bottomLeft:) 

Initializer

# init(topLeft:topRight:bottomRight:bottomLeft:)

Creates a rectangle observation from its corner points.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
init(
    topLeft: NormalizedPoint,
    topRight: NormalizedPoint,
    bottomRight: NormalizedPoint,
    bottomLeft: NormalizedPoint
)
```

## Discussion

The framework normalizes the coordinates of the rectangle to the dimensions of the processed image, with the origin at the bottom-left corner of the image.

## See Also

### Creating an observation

init(VNRectangleObservation)

Creates a rectangle observation.

