

- Create ML Components
-  SerializationError 

Enumeration

# SerializationError

A serialization error.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
enum SerializationError
```

## Topics

### Analyzing the error

case notRepresentableAsCoreML(debugDescription: String)

An error that indicates that the transformer cannot be represented as a CoreML model.

case packageAlreadyExists(URL)

An error that indicates that the package already exists at the URL.

case packageNotFound(URL)

An error that indicates that the package at specified URL was not found.

var errorDescription: String?

A localized message describing what error occurred.

### Operators

static func == (SerializationError, SerializationError) -> Bool

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

enum TabularPipelineDataError

Errors related to tabular pipeline data affinity problems.

enum VideoReaderError

Video loader errors.

