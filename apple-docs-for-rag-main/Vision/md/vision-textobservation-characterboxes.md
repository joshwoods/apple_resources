

- Vision
- TextObservation
-  characterBoxes 

Instance Property

# characterBoxes

An array of detected individual character bounding boxes.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
let characterBoxes: [RectangleObservation]?
```

## Discussion

If the associated DetectTextRectanglesRequest indicates interest in character boxes by setting the option reportCharacterBoxes to `true`, this property is non-`nil`. If no characters are found, it remains empty.

## See Also

### Inspecting an observation

struct RectangleObservation

An object that represents the four vertices of a detected rectangle.

