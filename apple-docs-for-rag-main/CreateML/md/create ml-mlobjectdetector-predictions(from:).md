

- Create ML
- MLObjectDetector
-  predictions(from:) 

Instance Method

# predictions(from:)

Locates objects in an array of images and generates an array of annotation collections, one for each input image.

macOS 10.15+

``` source
func predictions(from images: [URL]) throws -> [MLObjectDetector.DetectedObjects]
```

## Return Value

An MLObjectDetector.DetectedObjects array, where each element represents the annotations of the items the object detector found in the corresponding input image.

## Discussion

- images: An array of URLs for the image files where you want the object detector to look for objects.

## See Also

### Testing an object detector

func prediction(from: URL) throws -> MLObjectDetector.DetectedObjects

Locates objects in an image and generates an annotation for each object it detects.

typealias DetectedObjects

An array of annotations that represent the items an object detector found in an image.

struct ObjectAnnotation

The label, location, and confidence score of an item the object detector found in an image.

