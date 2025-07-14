

- Create ML Components
- BoostedTreeClassifier
-  fitted(to:validateOn:eventHandler:) 

Instance Method

# fitted(to:validateOn:eventHandler:)

Fits a boosted tree classifier model to a collection of examples.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func fitted(
    to input: DataFrame,
    validateOn validation: DataFrame? = nil,
    eventHandler: EventHandler? = nil
) async throws -> TreeClassifierModel
```

## Parameters 

`input`  

A data frame of examples.

`validation`  

A data frame of validation examples.

`eventHandler`  

An event handler. This method reports accuracy and loss metrics.

## Return Value

The fitted boosted tree classifier model.

## See Also

### Fitting the classifier

typealias Annotation

The annotation type.

typealias Transformer

The transformer type created by this estimator.

