

- Create ML Components
- LinearTimeSeriesForecaster
-  update(\_:with:eventHandler:) 

Instance Method

# update(\_:with:eventHandler:)

Updates a model with a sequence of features.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func update(
    _ model: inout LinearTimeSeriesForecaster.Model,
    with input: some Sequence, MLShapedArray>>,
    eventHandler: EventHandler? = nil
) async throws
```

Available when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

## Parameters 

`model`  

The model to update.

`input`  

A sequence of annotated features. The feature shape must be `[featureSize]` and the annotation shape must be `[annotationSize]`.

`eventHandler`  

An event handler.

## Discussion

This method uses a sliding window to chunk the input features into features of inputWindowSize elements and annotations of forecastWindowSize elements. If you want to use a different windowing strategy, use update(_:withWindows:eventHandler:).

