

- Create ML Components
- TimeSeriesClassifier
- TimeSeriesClassifier.Model
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Performs the transformation on an input sequence.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func applied(
    to input: some TemporalSequence>,
    eventHandler: EventHandler? = nil
) async throws -> AnyTemporalSequence>
```

Available when `Scalar` conforms to `MLShapedArrayScalar`, `Scalar` conforms to `BinaryFloatingPoint`, `Label` conforms to `Comparable`, `Label` conforms to `Decodable`, `Label` conforms to `Encodable`, and `Label` conforms to `Hashable`.

## Parameters 

`input`  

A temporal sequence of features. Each feature’s shape must be `[featureSize]`.

`eventHandler`  

An event handler.

## Return Value

An temporal sequence of predictions. Each prediction’s shape is `[forecastWindowSize, annotationSize]`.

