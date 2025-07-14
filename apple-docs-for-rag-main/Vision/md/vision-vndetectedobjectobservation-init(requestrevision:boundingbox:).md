

- Vision
- VNDetectedObjectObservation
-  init(requestRevision:boundingBox:) 

Initializer

# init(requestRevision:boundingBox:)

Creates an observation with a revision number and bounding box.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
convenience init(
    requestRevision: Int,
    boundingBox: CGRect
)
```

## Parameters 

`requestRevision`  

The revision of the request to use.

`boundingBox`  

The observation’s bounding box, in coordinates normalized to the dimensions of the processed image, with its origin at the image’s lower-left corner.

## See Also

### Creating an Observation

convenience init(boundingBox: CGRect)

Creates an observation with a bounding box.

