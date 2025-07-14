

- Create ML Components
- TimeSeriesClassifier
-  update(\_:with:eventHandler:) 

Instance Method

# update(\_:with:eventHandler:)

Updates a model with a new batch of examples.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func update(
    _ transformer: inout TimeSeriesClassifier.Model,
    with input: some Sequence, Label>>,
    eventHandler: EventHandler? = nil
) async throws
```

Available when `Scalar` conforms to `MLShapedArrayScalar`, `Scalar` conforms to `BinaryFloatingPoint`, `Label` conforms to `Comparable`, `Label` conforms to `Decodable`, `Label` conforms to `Encodable`, and `Label` conforms to `Hashable`.

## Parameters 

`transformer`  

A transformer to update.

`input`  

A sequence of annotated features for updating the transformer. Each feature’s shape should be `[sequenceLength, featureSize]`.

`eventHandler`  

An event handler.

