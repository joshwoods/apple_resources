

- Create ML Components
-  LinearTransformer 

Structure

# LinearTransformer

A transformer that runs an input through a scale and offset.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct LinearTransformer where Element : BinaryFloatingPoint, Element : Decodable, Element : Encodable
```

## Topics

### Creating a regressor

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

init(scale: Element, offset: Element)

Creates a linear transformer.

### Getting the properties

var offset: Element

The amount to be offset after scaling.

var scale: Element

The amount to be scaled.

### Performing the transformation

func applied&lt;S>(to: S, eventHandler: EventHandler?) -> [Element]

Scales a sequence of inputs.

func applied(to: Element, eventHandler: EventHandler?) -> Element

Scales an input.

### Operators

static func == (LinearTransformer&lt;Element>, LinearTransformer&lt;Element>) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

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
- Hashable
- Sendable
- Transformer

## See Also

### Preprocessors

struct ImputeTransformer

A transformer that replaces missing values with a pre-defined value.

struct OneHotEncoder

An estimator that encodes categorical values to an integer array.

struct OrdinalEncoder

An ordinal encoder estimator encodes categorical values to ordinal integer values.

struct NumericImputer

An estimator that replaces missing values in the numeric input.

struct Reshaper

A transformer that reshapes a shaped array.

struct CategoricalImputer

An estimator that replaces missing values in the categorical input.

struct OptionalUnwrapper

A transformer that unwraps optional elements and throws when encountering missing values.

