

- Create ML Components
-  ImputeTransformer 

Structure

# ImputeTransformer

A transformer that replaces missing values with a pre-defined value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct ImputeTransformer where Element : Decodable, Element : Encodable
```

## Topics

### Creating a transformer

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

init(value: Element)

Creates an impute transformer.

### Getting the impute value

var value: Element

Impute value used to replace missing values.

### Performing the transformation

func applied(to: Element?, eventHandler: EventHandler?) -> Element

Imputes a single input.

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

Hashable Implementations

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

struct LinearTransformer

A transformer that runs an input through a scale and offset.

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

