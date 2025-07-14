

- Create ML Components
- LinearTimeSeriesForecaster
-  update(\_:withWindows:eventHandler:) 

Instance Method

# update(\_:withWindows:eventHandler:)

Updates a model with a sequence of windows.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func update(
    _ model: inout LinearTimeSeriesForecaster.Model,
    withWindows windows: some Sequence, MLShapedArray>>,
    eventHandler: EventHandler? = nil
) async throws
```

Available when `Scalar` conforms to `MLShapedArrayScalar` and `BinaryFloatingPoint`.

## Parameters 

`model`  

The model to update.

`windows`  

A sequence of annotated windows. The feature shape must be `[inputWindowSize, featureSize]` and the annotation shape must be `[forecastWindowSize, annotationSize]`.

`eventHandler`  

An event handler.

## Discussion

For faster updates, consider passing a single AnnotatedBatch with shaped arrays that contain multiple training examples. See update(_:with:).

