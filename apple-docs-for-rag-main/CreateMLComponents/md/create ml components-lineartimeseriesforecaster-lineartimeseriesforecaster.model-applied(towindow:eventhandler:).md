

- Create ML Components
- LinearTimeSeriesForecaster
- LinearTimeSeriesForecaster.Model
-  applied(toWindow:eventHandler:) 

Instance Method

# applied(toWindow:eventHandler:)

Performs a prediction on a window of input features.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func applied(
    toWindow input: MLShapedArray,
    eventHandler: EventHandler? = nil
) async throws -> MLShapedArray
```

## Parameters 

`input`  

An window of input features with shape `[inputWindowSize, featureSize]`.

`eventHandler`  

An event handler.

## Return Value

A shaped array of predictions with shape `[forecastWindowSize, annotationSize]`.

