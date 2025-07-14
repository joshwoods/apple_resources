

- Create ML Components
-  CompatibilityError 

Enumeration

# CompatibilityError

A compatibility error.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
enum CompatibilityError
```

## Topics

### Analyzing the Error

case unsupportedRevision(Int)

An error that indicates that the revision is not supported.

var errorDescription: String?

A localized message describing what error occurred.

### Operators

static func == (CompatibilityError, CompatibilityError) -> Bool

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

enum TabularPipelineDataError

Errors related to tabular pipeline data affinity problems.

enum VideoReaderError

Video loader errors.

