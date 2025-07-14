

- Create ML
- MLObjectDetector
-  MLObjectDetector.DetectedObjects 

Type Alias

# MLObjectDetector.DetectedObjects

An array of annotations that represent the items an object detector found in an image.

macOS 10.15+

``` source
typealias DetectedObjects = [MLObjectDetector.ObjectAnnotation]
```

## See Also

### Testing an object detector

func prediction(from: URL) throws -> MLObjectDetector.DetectedObjects

Locates objects in an image and generates an annotation for each object it detects.

func predictions(from: [URL]) throws -> [MLObjectDetector.DetectedObjects]

Locates objects in an array of images and generates an array of annotation collections, one for each input image.

struct ObjectAnnotation

The label, location, and confidence score of an item the object detector found in an image.

