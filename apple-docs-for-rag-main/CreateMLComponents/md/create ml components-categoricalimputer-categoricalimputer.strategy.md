

- Create ML Components
- CategoricalImputer
-  CategoricalImputer.Strategy 

Enumeration

# CategoricalImputer.Strategy

An imputation strategy.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
enum Strategy
```

## Topics

### Imputer strategies

case constant(Element)

Imputation strategy that replaces missing elements with a constant.

case mode

Imputation strategy that replaces missing elements with the mode.

## Relationships

### Conforms To

- Sendable

## See Also

### Fitting

func fitted&lt;S>(to: S, eventHandler: EventHandler?) -> CategoricalImputer&lt;Element>.Transformer

Fits a categorical imputer to a sequence of elements.

typealias Transformer

The transformer type created by this estimator.

