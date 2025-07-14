

- Create ML Components
- SupervisedTemporalEstimator
-  fitted(to:eventHandler:) Deprecated

Instance Method

# fitted(to:eventHandler:)

Fits a transformer to a sequence of examples.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func fitted(
    to input: InputSequence,
    eventHandler: EventHandler?
) async throws -> Self.Transformer where InputSequence : Sequence, FeatureSequence : TemporalSequence, InputSequence.Element == AnnotatedFeature, FeatureSequence.Feature == Self.Transformer.Input
```

**Required**

## Parameters 

`input`  

A sequence of annotated temporal sequences used for fitting the transformer.

`eventHandler`  

An event handler.

## Return Value

The fitted transformer.

## See Also

### Fitting

func fitted&lt;InputSequence, FeatureSequence>(to: InputSequence) async throws -> Self.TransformerDeprecated

func fitted&lt;InputSequence, Validation, FeatureSequence>(to: InputSequence, validateOn: Validation) async throws -> Self.TransformerDeprecated

func fitted&lt;InputSequence, Validation, FeatureSequence>(to: InputSequence, validateOn: Validation, eventHandler: EventHandler?) async throws -> Self.Transformer

Fits a transformer to a sequence of examples while validating with a validation sequence.

**Required**

Deprecated

associatedtype Annotation : Equatable, Sendable

The annotation type.

**Required**

Deprecated

associatedtype Transformer : TemporalTransformer

The transformer type created by this estimator.

**Required**

Deprecated

