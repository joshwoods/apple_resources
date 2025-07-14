

- Vision
- TrackRectangleRequest
-  init(detectedRectangle:\_:frameAnalysisSpacing:) 

Initializer

# init(detectedRectangle:\_:frameAnalysisSpacing:)

Creates a rectangle tracking request.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
init(
    detectedRectangle: any QuadrilateralProviding & VisionObservation,
    _ revision: TrackRectangleRequest.Revision? = nil,
    frameAnalysisSpacing: CMTime? = nil
)
```

