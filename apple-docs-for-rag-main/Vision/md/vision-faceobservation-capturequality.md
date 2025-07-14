

- Vision
- FaceObservation
-  captureQuality 

Instance Property

# captureQuality

The quality of the face capture.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
let captureQuality: FaceObservation.CaptureQuality?
```

## Discussion

This value is nil for face observations produced by a `DetectFaceRectanglesRequest` analysis. Use DetectFaceCaptureQualityRequest to detect capture quality.

