

- Create ML Components
-  OrdinalEncoder 

Structure

# OrdinalEncoder

An ordinal encoder estimator encodes categorical values to ordinal integer values.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct OrdinalEncoder where Category : Comparable, Category : Decodable, Category : Encodable, Category : Hashable
```

## Topics

### Creating an encoder

init()

Creates an ordinal encoding estimator.

### Fitting

func fitted&lt;S>(to: S, eventHandler: EventHandler?) throws -> OrdinalEncoder&lt;Category>.Transformer

Fits an ordinal encoder to a sequence of categories.

### Default Implementations

Estimator Implementations

UpdatableEstimator Implementations

## Relationships

### Conforms To

- Copyable
- Estimator
- Sendable
- UpdatableEstimator

  Conforms when `Category` conforms to `Comparable`, `Decodable`, `Encodable`, and `Hashable`.

## See Also

### Preprocessors

struct LinearTransformer

A transformer that runs an input through a scale and offset.

struct ImputeTransformer

A transformer that replaces missing values with a pre-defined value.

struct OneHotEncoder

An estimator that encodes categorical values to an integer array.

struct NumericImputer

An estimator that replaces missing values in the numeric input.

struct Reshaper

A transformer that reshapes a shaped array.

struct CategoricalImputer

An estimator that replaces missing values in the categorical input.

struct OptionalUnwrapper

A transformer that unwraps optional elements and throws when encountering missing values.

