

- Create ML
- MLObjectDetector
- MLObjectDetector.ObjectAnnotation
-  confidence 

Instance Property

# confidence

The object detector’s confidence score for its prediction’s accuracy.

macOS 10.15+

``` source
var confidence: Double
```

## Discussion

The confidence range is `[0.0, 1.0]`, where `1.0` is the highest possible confidence score.

## See Also

### Inspecting an annotation

var label: String

The name of the item the object detector found in an image.

var boundingBox: CGRect

A rectangular region that encloses an item the object detector found in the image.

