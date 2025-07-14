

- Create ML Components
- LinearTimeSeriesForecaster
- LinearTimeSeriesForecaster.Model
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Performs a prediction on a shaped array of features.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func applied(
    to input: MLShapedArray,
    eventHandler: EventHandler? = nil
) async throws -> MLShapedArray
```

## Parameters 

`input`  

An shaped array of features. The shape must be `[N, featureSize]` where `N` is the length of the sequence, which must be at least `inputWindowSize`.

`eventHandler`  

An event handler.

## Return Value

A shaped array of predictions with shape `[M, forecastWindowSize, annotationSize]` where `M` is the number of predictions based on the input sequence length and the stride property.

## Discussion

This method uses a sliding window to chunk the input features into inputWindowSize elements every stride elements. If you want to use a different windowing strategy, use applied(toWindow:eventHandler:).

