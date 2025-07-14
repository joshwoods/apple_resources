

- Create ML Components
- MLModelImageFeatureExtractor
-  MLModelImageFeatureExtractor.Error 

Enumeration

# MLModelImageFeatureExtractor.Error

CoreML Extraction error.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
enum Error
```

## Topics

### Analyzing the error

case invalidInput(String)

An error indicating that the mlmodel does not take required input.

case invalidOutput(String)

An error indicating that the mlmodel does not produce the required output.

var debugDescription: String

A text representation of the error.

### Operators

static func == (MLModelImageFeatureExtractor.Error, MLModelImageFeatureExtractor.Error) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

Equatable Implementations

Error Implementations

## Relationships

### Conforms To

- CustomDebugStringConvertible
- Equatable
- Error
- Sendable

## See Also

### Applying

func applied(to: CIImage, eventHandler: EventHandler?) async throws -> MLShapedArray&lt;Float>

Uses the CoreML model to create image features from the input pixel buffer.

