

- Create ML
- MLObjectDetector
-  MLObjectDetector.ObjectAnnotation 

Structure

# MLObjectDetector.ObjectAnnotation

The label, location, and confidence score of an item the object detector found in an image.

macOS 10.15+

``` source
struct ObjectAnnotation
```

## Topics

### Creating an annotation

init(label: String, boundingBox: CGRect, confidence: Double)

Creates an annotation for an item an object detector finds in an image.

### Inspecting an annotation

var label: String

The name of the item the object detector found in an image.

var boundingBox: CGRect

A rectangular region that encloses an item the object detector found in the image.

var confidence: Double

The object detector’s confidence score for its prediction’s accuracy.

### Describing an annotation

var description: String

A text representation of the object annotation.

var debugDescription: String

A text representation of the object annotation that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the object annotation within a playground.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomPlaygroundDisplayConvertible Implementations

CustomStringConvertible Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomPlaygroundDisplayConvertible
- CustomStringConvertible
- Sendable

## See Also

### Testing an object detector

func prediction(from: URL) throws -> MLObjectDetector.DetectedObjects

Locates objects in an image and generates an annotation for each object it detects.

func predictions(from: [URL]) throws -> [MLObjectDetector.DetectedObjects]

Locates objects in an array of images and generates an array of annotation collections, one for each input image.

typealias DetectedObjects

An array of annotations that represent the items an object detector found in an image.

