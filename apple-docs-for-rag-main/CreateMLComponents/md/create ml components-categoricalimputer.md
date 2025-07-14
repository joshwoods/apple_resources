

- Create ML Components
-  CategoricalImputer 

Structure

# CategoricalImputer

An estimator that replaces missing values in the categorical input.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct CategoricalImputer where Element : Decodable, Element : Encodable, Element : Hashable
```

## Topics

### Creating an estimator

init(CategoricalImputer&lt;Element>.Strategy)

Creates an imputer with a strategy.

init(constant: Element)

Creates an imputer with a constant value to use when replacing missing values.

### Getting the properties

var strategy: CategoricalImputer&lt;Element>.Strategy

The imputation strategy.

### Fitting

func fitted&lt;S>(to: S, eventHandler: EventHandler?) -> CategoricalImputer&lt;Element>.Transformer

Fits a categorical imputer to a sequence of elements.

typealias Transformer

The transformer type created by this estimator.

enum Strategy

An imputation strategy.

### Default Implementations

CustomDebugStringConvertible Implementations

Estimator Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Estimator
- Sendable

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

struct OptionalUnwrapper

A transformer that unwraps optional elements and throws when encountering missing values.

