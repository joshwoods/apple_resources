

- Create ML Components
-  AudioPreprocessingError 

Enumeration

# AudioPreprocessingError

Audio preprocessing errors.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
enum AudioPreprocessingError
```

## Topics

### Analyzing the error

case incompatibleTargetFormatForConversion(inputFormat: AVAudioFormat, targetFormat: AVAudioFormat)

An error that indicates that the input and output formats are incompatible for creating an audio converter.

var errorDescription: String?

A localized message describing what error occurred.

### Operators

static func == (AudioPreprocessingError, AudioPreprocessingError) -> Bool

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

enum TabularPipelineDataError

Errors related to tabular pipeline data affinity problems.

enum VideoReaderError

Video loader errors.

