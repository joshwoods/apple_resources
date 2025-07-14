

- Vision
- VNDetectTextRectanglesRequest
-  reportCharacterBoxes 

Instance Property

# reportCharacterBoxes

A Boolean value that indicates whether the request detects character bounding boxes.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var reportCharacterBoxes: Bool { get set }
```

## Discussion

Set the value to true to have the detector return character bounding boxes as an array of VNRectangleObservation objects.

