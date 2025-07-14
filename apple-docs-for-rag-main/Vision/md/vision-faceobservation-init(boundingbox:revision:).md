

- Vision
- FaceObservation
-  init(boundingBox:revision:) 

Initializer

# init(boundingBox:revision:)

Creates a face observation from its bounding box.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
init(
    boundingBox: NormalizedRect,
    revision: DetectFaceRectanglesRequest.Revision? = nil
)
```

## Parameters 

`boundingBox`  

The bounding box of the detected face.

`revision`  

The revision of the DetectFaceRectanglesRequest that provided the bounding box.

## See Also

### Creating an observation

init(VNFaceObservation)

Creates a face observation.

