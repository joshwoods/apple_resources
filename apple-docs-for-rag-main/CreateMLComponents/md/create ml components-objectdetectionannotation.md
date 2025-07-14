

- Create ML Components
-  ObjectDetectionAnnotation 

Structure

# ObjectDetectionAnnotation

An object detection annotation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
struct ObjectDetectionAnnotation where Label : Comparable, Label : Decodable, Label : Encodable, Label : Hashable
```

## Overview

The annotation consists of a list of bounding boxes and object labels for each image.

## Topics

### Creating an annotation

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Getting the properties

let imageFileName: String

The name of the image file.

let objects: [ObjectDetectionAnnotation&lt;Label>.Annotation]

The list of object annotations in the image.

struct Annotation

The annotation represented by an object label and its bounding box.

let prominentObject: Label

The most prominent object in the image.

### Encoding and decoding

enum CodingKeys

Coding keys for object detection annotations

### Operators

static func == (ObjectDetectionAnnotation&lt;Label>, ObjectDetectionAnnotation&lt;Label>) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

Equatable Implementations

Identifiable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Equatable
- Identifiable
- Sendable

## See Also

### Object detection components

struct DetectedObject

An item in a detection result.

struct ObjectDetectionMetrics

Metrics for object detection model.

