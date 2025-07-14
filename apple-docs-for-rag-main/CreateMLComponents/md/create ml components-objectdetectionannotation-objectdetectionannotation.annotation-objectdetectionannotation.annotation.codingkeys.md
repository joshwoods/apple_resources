

- Create ML Components
- ObjectDetectionAnnotation
- ObjectDetectionAnnotation.Annotation
-  ObjectDetectionAnnotation.Annotation.CodingKeys 

Enumeration

# ObjectDetectionAnnotation.Annotation.CodingKeys

Coding keys for Annotation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
enum CodingKeys
```

## Topics

### Coding keys

case boundingBox

case label

### Creating a key

init?(intValue: Int)

Creates a new instance from the specified integer.

init?(rawValue: String)

Creates a new instance with the specified raw value.

init?(stringValue: String)

Creates a new instance from the given string.

### Instance Properties

var intValue: Int?

The value to use in an integer-indexed collection (e.g. an int-keyed dictionary).

var rawValue: String

The corresponding value of the raw type.

var stringValue: String

The string to use in a named collection (e.g. a string-keyed dictionary).

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

CodingKey Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- CodingKey
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- RawRepresentable
- Sendable

