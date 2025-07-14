

- Create ML Components
- TimeSeriesClassifier
- TimeSeriesClassifier.Model
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Performs a classification on a shaped array of input features.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func applied(
    to input: MLShapedArray,
    eventHandler: EventHandler? = nil
) async throws -> ClassificationDistribution
```

## Parameters 

`input`  

A shaped array of input features. The shape must `[sequenceLength, featureSize]`.

`eventHandler`  

An event handler.

## Return Value

A classification distribution.

