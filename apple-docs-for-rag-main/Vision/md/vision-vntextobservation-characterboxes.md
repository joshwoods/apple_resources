

- Vision
- VNTextObservation
-  characterBoxes 

Instance Property

# characterBoxes

An array of detected individual character bounding boxes.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var characterBoxes: [VNRectangleObservation]? { get }
```

## Discussion

If the associated VNDetectTextRectanglesRequest request indicates interest in character boxes by setting the option `reportCharacterBoxes` to true, this property is non-`nil`. If no characters are found, it remains empty.

