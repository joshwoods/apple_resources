

- Vision
- DetectFaceCaptureQualityRequest
-  inputFaceObservations 

Instance Property

# inputFaceObservations

An array of face-observation objects to process as part of the request.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var inputFaceObservations: [FaceObservation]?
```

## Discussion

The default is `nil`. When `nil`, the framework first performs a DetectFaceRectanglesRequest and processes all faces detected.

