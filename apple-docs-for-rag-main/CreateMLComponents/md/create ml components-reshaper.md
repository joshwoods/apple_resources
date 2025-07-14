

- Create ML Components
-  Reshaper 

Structure

# Reshaper

A transformer that reshapes a shaped array.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct Reshaper where Scalar : MLShapedArrayScalar, Scalar : Decodable, Scalar : Encodable
```

## Topics

### Creating a transformer

init(shape: [Int])

Creates a reshape transformer.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Getting the shape

var shape: [Int]

The target shape.

### Performing the transformation

func applied&lt;S>(S, eventHandler: EventHandler?) throws -> [MLShapedArray&lt;Scalar>]

Reshapes a sequence of inputs.

func applied(to: MLShapedArray&lt;Scalar>, eventHandler: EventHandler?) throws -> MLShapedArray&lt;Scalar>

Reshapes the input.

### Operators

static func == (Reshaper&lt;Scalar>, Reshaper&lt;Scalar>) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

### Type Aliases

typealias Input

The input type.

typealias Output

The output type.

### Default Implementations

CustomDebugStringConvertible Implementations

Equatable Implementations

Transformer Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Decodable
- Encodable
- Equatable
- Sendable
- Transformer

## See Also

### Preprocessors

struct LinearTransformer

A transformer that runs an input through a scale and offset.

struct ImputeTransformer

A transformer that replaces missing values with a pre-defined value.

struct OneHotEncoder

An estimator that encodes categorical values to an integer array.

struct OrdinalEncoder

An ordinal encoder estimator encodes categorical values to ordinal integer values.

struct NumericImputer

An estimator that replaces missing values in the numeric input.

struct CategoricalImputer

An estimator that replaces missing values in the categorical input.

struct OptionalUnwrapper

A transformer that unwraps optional elements and throws when encountering missing values.

