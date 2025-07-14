

- Create ML
- MLProgress
-  MLProgress.Metric 

Enumeration

# MLProgress.Metric

Metrics you use to evaluate a model’s performance during a training session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
enum Metric
```

## Topics

### Retrieving metric keys

case accuracy

The metric for the model’s accuracy.

case contentLoss

The metric for the style transfer model’s content loss.

case loss

The metric for the model’s loss.

case maximumError

The metric for the model’s maximum error.

case rootMeanSquaredError

The metric for the model’s root mean squared error (RMSE).

case styleLoss

The metric for the style transfer model’s style loss.

case stylizedImageURL

The location of the stylized image content in the file system.

case validationAccuracy

The metric for the model’s validation accuracy.

case validationLoss

The metric for the model’s validation loss.

case validationMaximumError

The metric for the model’s validation maximum error.

case validationRootMeanSquaredError

The metric for the model’s validation root mean squared error (RMSE).

### Iterating all metric keys

static var allCases: [MLProgress.Metric]

A collection of all values of this type.

typealias AllCases

A type that can represent a collection of all values of this type.

### Creating a key from a string

init?(rawValue: String)

Creates a new instance with the specified raw value.

### Getting a key’s string value

var rawValue: String

The corresponding value of the raw type.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Encoding and decoding a key

func encode(to: any Encoder) throws

Encodes this value into the given encoder, when the type’s `RawValue` is `String`.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder, when the type’s `RawValue` is `String`.

### Providing a key’s hash value

func hash(into: inout Hasher)

var hashValue: Int

### Comparing metric keys

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- CaseIterable
- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Assessing a checkpoint

var metrics: [MLProgress.Metric : Any]

Measurements of the model’s performance at the time the session saved the checkpoint.

