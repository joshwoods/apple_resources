

- Create ML Components
- NumericImputer
-  fitted(to:eventHandler:) 

Instance Method

# fitted(to:eventHandler:)

Fits a numeric imputer to a sequence of elements.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func fitted(
    to input: S,
    eventHandler: EventHandler? = nil
) -> NumericImputer.Transformer where S : Sequence, S.Element == Element?
```

## Parameters 

`input`  

A sequence of elements.

`eventHandler`  

An event handler.

## Return Value

The fitted transformer.

## See Also

### Fitting

typealias Transformer

The transformer type created by this estimator.

enum Strategy

An imputation strategy.

