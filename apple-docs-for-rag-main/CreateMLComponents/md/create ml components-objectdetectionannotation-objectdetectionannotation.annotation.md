

- Create ML Components
- ObjectDetectionAnnotation
-  ObjectDetectionAnnotation.Annotation 

Structure

# ObjectDetectionAnnotation.Annotation

The annotation represented by an object label and its bounding box.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
struct Annotation
```

## Topics

### Getting the properties

let boundingBox: CGRect

The bounding box that describes the spatial location of the object.

let label: Label

The object label.

### Encoding and decoding

enum CodingKeys

Coding keys for Annotation.

### Operators

static func == (ObjectDetectionAnnotation&lt;Label>.Annotation, ObjectDetectionAnnotation&lt;Label>.Annotation) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

Decodable Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Equatable
- Sendable

## See Also

### Getting the properties

let imageFileName: String

The name of the image file.

let objects: [ObjectDetectionAnnotation&lt;Label>.Annotation]

The list of object annotations in the image.

let prominentObject: Label

The most prominent object in the image.

