

- Create ML
-  MLPhase 

Enumeration

# MLPhase

The possible states of a training session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
enum MLPhase
```

## Topics

### Retrieving session phases

case initialized

The training session is in the initial idle state before extracting features and training.

case extractingFeatures

The training session is extracting features from the training dataset.

case training

The training session is training a model from the features it extracted from the training dataset.

case evaluating

The training session is evaluating the model it trained.

case inferencing

The training session is using the model to make a prediction.

### Creating a phase from a string

init?(rawValue: String)

Creates a new instance with the specified raw value.

### Getting a phase’s string value

var rawValue: String

The corresponding value of the raw type.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Encoding and decoding a phase

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `String`.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder, when the type’s `RawValue` is `String`.

### Providing a phase’s hash value

func hash(into: inout Hasher)

var hashValue: Int

### Comparing phases

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Checking a training session’s progress

var phase: MLPhase

The training session’s current state.

var iteration: Int

The iteration number of a training session’s phase.

var checkpoints: [MLCheckpoint]

An array of checkpoints the training session has created so far.

