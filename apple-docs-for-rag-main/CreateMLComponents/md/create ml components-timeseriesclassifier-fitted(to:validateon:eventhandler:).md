

- Create ML Components
- TimeSeriesClassifier
-  fitted(to:validateOn:eventHandler:) 

Instance Method

# fitted(to:validateOn:eventHandler:)

Fits a time series classifier model to a sequence of examples.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func fitted(
    to input: some Sequence, Label>>,
    validateOn validation: some Sequence, Label>>,
    eventHandler: EventHandler? = nil
) async throws -> TimeSeriesClassifier.Model
```

## Parameters 

`input`  

A sequence of annotated features for training. Each feature’s shape should be `[sequenceLength, featureSize]`.

`validation`  

A sequence of annotated features for validating. Each feature’s shape should be `[sequenceLength, featureSize]`.

`eventHandler`  

An event handler.

## Return Value

The fitted time series classifier model.

## Discussion

The training process partitions the input into random batches according to the batch size configuration parameter. Training stops when the validation loss stops improving or when the maximum number of iterations is reached.

