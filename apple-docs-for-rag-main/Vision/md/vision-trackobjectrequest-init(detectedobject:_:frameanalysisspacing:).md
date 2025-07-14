

- Vision
- TrackObjectRequest
-  init(detectedObject:\_:frameAnalysisSpacing:) 

Initializer

# init(detectedObject:\_:frameAnalysisSpacing:)

Creates an object tracking request.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
init(
    detectedObject: any BoundingBoxProviding & VisionObservation,
    _ revision: TrackObjectRequest.Revision? = nil,
    frameAnalysisSpacing: CMTime? = nil
)
```

## See Also

### Creating a request

protocol BoundingBoxProviding

A protocol for objects that have a bounding box.

