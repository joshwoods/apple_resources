

- Create ML
- MLObjectDetector
-  prediction(from:) 

Instance Method

# prediction(from:)

Locates objects in an image and generates an annotation for each object it detects.

macOS 10.15+

``` source
func prediction(from image: URL) throws -> MLObjectDetector.DetectedObjects
```

## Return Value

An MLObjectDetector.DetectedObjects instance — which is an MLObjectDetector.ObjectAnnotation array — where each annotation represents an item the object detector found in the image.

## Discussion

- image: The URL for the image file where you want the object detector to look for objects.

## See Also

### Testing an object detector

func predictions(from: [URL]) throws -> [MLObjectDetector.DetectedObjects]

Locates objects in an array of images and generates an array of annotation collections, one for each input image.

typealias DetectedObjects

An array of annotations that represent the items an object detector found in an image.

struct ObjectAnnotation

The label, location, and confidence score of an item the object detector found in an image.

