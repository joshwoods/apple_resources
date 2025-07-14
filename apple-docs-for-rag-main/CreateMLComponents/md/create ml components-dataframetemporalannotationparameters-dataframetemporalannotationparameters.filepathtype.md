

- Create ML Components
- DataFrameTemporalAnnotationParameters
-  DataFrameTemporalAnnotationParameters.FilePathType 

Enumeration

# DataFrameTemporalAnnotationParameters.FilePathType

The file path type to be used.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
enum FilePathType
```

## Topics

### File path types

case absolute

The file path is absolute.

case relative(baseURL: URL)

The file path is relative to the `baseURL`.

### Getting the description

var description: String

A textual representation of this instance.

### Operators

static func == (DataFrameTemporalAnnotationParameters&lt;Annotation>.FilePathType, DataFrameTemporalAnnotationParameters&lt;Annotation>.FilePathType) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Sendable

