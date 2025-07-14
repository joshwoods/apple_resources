

- Create ML Components
-  TabularPipelineDataError 

Enumeration

# TabularPipelineDataError

Errors related to tabular pipeline data affinity problems.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
enum TabularPipelineDataError
```

## Topics

### Getting the cases

case incorrectType(operation: String, columnName: String, actual: String, expected: String)

A column has an incorrect type.

case missingColumn(operation: String, columnName: String)

A column is missing from the data frame.

case missingValues(operation: String, columnName: String)

The selected column has missing values.

var errorDescription: String?

A localized message describing what error occurred.

### Operators

static func == (TabularPipelineDataError, TabularPipelineDataError) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

CustomDebugStringConvertible Implementations

Equatable Implementations

Error Implementations

LocalizedError Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Equatable
- Error
- LocalizedError
- Sendable

## See Also

### Errors

enum AudioPreprocessingError

Audio preprocessing errors.

enum AudioReaderError

Audio reader errors.

enum CompatibilityError

A compatibility error.

enum ConcatenationError

Errors thrown when concatenating numeric values.

enum DatasetError

Dataset processing errors.

enum EstimatorEncodingError

An estimator encoding error.

enum ModelCompatibilityError

Errors related to CoreML model compatibility.

enum ModelUpdateError

An updatable model error.

enum OptimizationError

An optimization error.

enum PipelineDataError

Errors related to pipeline data affinity problems.

enum SerializationError

A serialization error.

enum VideoReaderError

Video loader errors.

