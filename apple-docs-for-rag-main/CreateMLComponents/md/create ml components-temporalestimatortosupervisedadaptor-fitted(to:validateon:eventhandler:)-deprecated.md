

- Create ML Components
- TemporalEstimatorToSupervisedAdaptor
-  fitted(to:validateOn:eventHandler:) Deprecated

Instance Method

# fitted(to:validateOn:eventHandler:)

Fits a transformer to a sequence of examples while validating with a validation sequence.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func fitted(
    to input: InputSequence,
    validateOn validation: Validation,
    eventHandler: EventHandler? = nil
) async throws -> TemporalEstimatorToSupervisedAdaptor.Transformer where InputSequence : Sequence, Validation : Sequence, FeatureSequence : TemporalSequence, InputSequence.Element == AnnotatedFeature, Validation.Element == AnnotatedFeature, FeatureSequence.Feature == Estimator.Transformer.Input
```

## Parameters 

`input`  

A sequence of examples used for fitting the transformer.

`validation`  

A sequence of examples used for validating the fitted transformer.

`eventHandler`  

An event handler.

## Return Value

The fitted transformer.

## See Also

### Fitting

func fitted&lt;InputSequence, FeatureSequence>(to: InputSequence, eventHandler: EventHandler?) async throws -> TemporalEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Fits a transformer to a sequence of examples.

Deprecated

typealias Transformer

The transformer type created by this estimator.

Deprecated

