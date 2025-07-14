

- Vision
- VNDetectedObjectObservation
-  boundingBox 

Instance Property

# boundingBox

The bounding box of the object that the request detects.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var boundingBox: CGRect { get }
```

## Discussion

The system normalizes the coordinates to the dimensions of the processed image, with the origin at the lower-left corner of the image.

