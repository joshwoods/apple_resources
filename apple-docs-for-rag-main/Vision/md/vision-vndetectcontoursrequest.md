

- Vision
-  VNDetectContoursRequest 

Class

# VNDetectContoursRequest

A request that detects the contours of the edges of an image.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class VNDetectContoursRequest
```

## Topics

### Configuring the Request

var contrastAdjustment: Float

The amount by which to adjust the image contrast.

var contrastPivot: NSNumber?

The pixel value to use as a pivot for the contrast.

var detectsDarkOnLight: Bool

A Boolean value that indicates whether the request detects a dark object on a light background to aid in detection.

var maximumImageDimension: Int

The maximum image dimension to use for contour detection.

var detectDarkOnLight: Bool

A Boolean value that indicates whether the request detects a dark object on a light background.

Deprecated

### Accessing the Results

var results: [VNContoursObservation]?

The results of the request to detect contours.

class VNContoursObservation

An object that represents the detected contours in an image.

### Identifying Request Revisions

let VNDetectContourRequestRevision1: Int

A constant for specifying revision 1 of the contours detection request.

## Relationships

### Inherits From

- VNImageBasedRequest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

