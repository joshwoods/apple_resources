

- Create ML Components
- PipelineDataError
-  PipelineDataError.incompatibleShape(\_:debugDescription:) 

Case

# PipelineDataError.incompatibleShape(\_:debugDescription:)

An error that indicates that an input’s doesn’t have the expected shape for the operation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
case incompatibleShape([
    Int],
    debugDescription: String
)
```

## See Also

### Analyzing the error

case emptyInput(operation: String)

An error that indicates that the input to fit is empty.

case incompatibleConfiguration(operation: String, debugDescription: String)

An error that indicates that an input is not compatible with an operation’s configuration.

case incompatibleDataFormat(operation: String, debugDescription: String)

An error that indicates that an input doesn’t have the expected data format.

case missingAnnotation(operation: String)

An error that indicates that an expected annotation is missing.

case missingValue(operation: String)

An error that indicates that an expected value is missing.

case unrecognizedCategory(operation: String, category: String)

An error that indicates that a new category was encountered after fitting.

var errorDescription: String?

A localized message describing what error occurred.

