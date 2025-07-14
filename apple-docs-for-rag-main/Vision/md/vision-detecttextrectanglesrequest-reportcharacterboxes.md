

- Vision
- DetectTextRectanglesRequest
-  reportCharacterBoxes 

Instance Property

# reportCharacterBoxes

A Boolean value that indicates whether the request detects character-bounding boxes.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var reportCharacterBoxes: Bool
```

## Discussion

Set the value to `true` to have the detector return character-bounding boxes as an array of VNRectangleObservation objects.

