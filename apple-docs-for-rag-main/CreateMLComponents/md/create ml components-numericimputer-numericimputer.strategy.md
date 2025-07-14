

- Create ML Components
- NumericImputer
-  NumericImputer.Strategy 

Enumeration

# NumericImputer.Strategy

An imputation strategy.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
enum Strategy
```

## Topics

### Imputer strategies

case constant(Element)

Imputation strategy that replaces missing elements with a constant.

case mean

Imputation strategy that replaces missing elements with the mean.

case median

Imputation strategy that replaces missing elements with the median.

## Relationships

### Conforms To

- Sendable

## See Also

### Fitting

func fitted&lt;S>(to: S, eventHandler: EventHandler?) -> NumericImputer&lt;Element>.Transformer

Fits a numeric imputer to a sequence of elements.

typealias Transformer

The transformer type created by this estimator.

