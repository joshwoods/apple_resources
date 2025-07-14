

- Vision
- VNDetectedObjectObservation
-  init(boundingBox:) 

Initializer

# init(boundingBox:)

Creates an observation with a bounding box.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
convenience init(boundingBox: CGRect)
```

## Parameters 

`boundingBox`  

The observation’s bounding box, in coordinates normalized to the dimensions of the processed image, with its origin at the image’s lower-left corner.

## See Also

### Creating an Observation

convenience init(requestRevision: Int, boundingBox: CGRect)

Creates an observation with a revision number and bounding box.

