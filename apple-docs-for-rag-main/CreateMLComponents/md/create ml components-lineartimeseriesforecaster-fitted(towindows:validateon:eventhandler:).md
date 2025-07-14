

- Create ML Components
- LinearTimeSeriesForecaster
-  fitted(toWindows:validateOn:eventHandler:) 

Instance Method

# fitted(toWindows:validateOn:eventHandler:)

Fits a model to a sequence of annotated windows with validation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func fitted(
    toWindows input: some Sequence, MLShapedArray>>,
    validateOn validation: some Sequence, MLShapedArray>>,
    eventHandler: EventHandler? = nil
) async throws -> LinearTimeSeriesForecaster.Model
```

## Parameters 

`input`  

A sequence of annotated windows. Each window’s shape should be `[inputWindowSize, featureSize]` and each annotation’s shape should be `[forecastWindowSize, annotationSize]`.

`validation`  

A sequence of annotated validation windows. The feature and annotation shapes should be the same as the input parameter.

`eventHandler`  

An event handler.

## Return Value

The fitted model.

