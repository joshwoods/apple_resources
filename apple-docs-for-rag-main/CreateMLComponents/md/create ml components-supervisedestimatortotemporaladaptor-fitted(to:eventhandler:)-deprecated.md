

- Create ML Components
- SupervisedEstimatorToTemporalAdaptor
-  fitted(to:eventHandler:) Deprecated

Instance Method

# fitted(to:eventHandler:)

Fits a transformer to a sequence of examples.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func fitted(
    to input: InputSequence,
    eventHandler: EventHandler? = nil
) async throws -> SupervisedEstimatorToTemporalAdaptor.Transformer where InputSequence : Sequence, FeatureSequence : TemporalSequence, InputSequence.Element == AnnotatedFeature, FeatureSequence.Feature == Base.Transformer.Input
```

## Parameters 

`input`  

A sequence of examples used for fitting the transformer.

`eventHandler`  

An event handler.

## Return Value

The fitted transformer.

## See Also

### Fitting

func fitted&lt;InputSequence, Validation, FeatureSequence>(to: InputSequence, validateOn: Validation, eventHandler: EventHandler?) async throws -> SupervisedEstimatorToTemporalAdaptor&lt;Base>.Transformer

Fits a transformer to a sequence of examples while validating with a validation sequence.

Deprecated

typealias Annotation

The annotation type.

Deprecated

typealias Input

The input type.

Deprecated

typealias Output

The output type.

Deprecated

typealias Transformer

The transformer type created by this estimator.

Deprecated

