

- Create ML Components
- LinearTimeSeriesForecaster
-  fitted(to:validateOn:eventHandler:) 

Instance Method

# fitted(to:validateOn:eventHandler:)

Fits a model to a sequence of examples with validation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func fitted(
    to input: some Sequence, MLShapedArray>>,
    validateOn validation: some Sequence, MLShapedArray>>,
    eventHandler: EventHandler? = nil
) async throws -> LinearTimeSeriesForecaster.Model
```

## Parameters 

`input`  

A sequence of annotated features. Each feature’s shape should be `[featureSize]` and each annotation’s shape should be `[annotationSize]`.

`validation`  

A sequence of annotated validation features. The feature and annotation shapes should be the same as the input parameter.

`eventHandler`  

An event handler.

## Return Value

The fitted model.

## Discussion

This method uses a sliding window to chunk the input features and validation features into features of inputWindowSize elements and annotations of forecastWindowSize elements. If you want to use a different windowing strategy, use fitted(toWindows:validateOn:eventHandler:).

