

- Create ML Components
-  OptionalUnwrapper 

Structure

# OptionalUnwrapper

A transformer that unwraps optional elements and throws when encountering missing values.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct OptionalUnwrapper
```

## Topics

### Creating a transformer

init()

Creates a transformer that unwraps an optional element or throws if the value is nil.

### Performing the transformation

func applied(to: Element?, eventHandler: EventHandler?) throws -> Element

Unwraps an optional element or throws if the value is `nil`.

### Type Aliases

typealias Input

The input type.

typealias Output

The output type.

### Default Implementations

Transformer Implementations

## Relationships

### Conforms To

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

struct Reshaper

A transformer that reshapes a shaped array.

struct CategoricalImputer

An estimator that replaces missing values in the categorical input.

