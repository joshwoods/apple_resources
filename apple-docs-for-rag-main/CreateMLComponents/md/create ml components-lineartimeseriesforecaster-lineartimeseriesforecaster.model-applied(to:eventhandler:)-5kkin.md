

- Create ML Components
- LinearTimeSeriesForecaster
- LinearTimeSeriesForecaster.Model
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Performs a prediction on a sequence of input features.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func applied(
    to input: some Sequence>,
    eventHandler: EventHandler? = nil
) async throws -> [MLShapedArray]
```

## Parameters 

`input`  

An sequence of input features. Each feature’s shape must be `[featureSize]`. If the sequence contains less than inputWindowSize elements the method returns an empty array.

`eventHandler`  

An event handler.

## Return Value

An array of predictions. Each prediction’s shape is `[forecastWindowSize, annotationSize]`. The number of predictions depends on the input sequence length and the stride property.

## Discussion

This method uses a sliding window to chunk the input features into inputWindowSize elements every stride elements. If you want to use a different windowing strategy, use applied(toWindow:eventHandler:).

