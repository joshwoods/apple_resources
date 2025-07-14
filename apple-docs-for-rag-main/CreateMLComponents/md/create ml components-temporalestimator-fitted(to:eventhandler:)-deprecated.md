

- Create ML Components
- TemporalEstimator
-  fitted(to:eventHandler:) Deprecated

Instance Method

# fitted(to:eventHandler:)

Fits a transformer to a sequence of examples.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func fitted(
    to input: InputSequence,
    eventHandler: EventHandler?
) async throws -> Self.Transformer where InputSequence : Sequence, InputSequence.Element : TemporalSequence, Self.Transformer.Input == InputSequence.Element.Feature
```

**Required**

## Parameters 

`input`  

A sequence of examples.

`eventHandler`  

An event handler.

## Return Value

The fitted transformer.

## See Also

### Adapting and fitting

func adaptedAsSupervised&lt;Annotation>(annotationType: Annotation.Type) -> TemporalEstimatorToSupervisedAdaptor&lt;Self, Annotation>

Exposes this temporal estimator as a supervised temporal estimator.

Deprecated

func fitted&lt;InputSequence>(to: InputSequence) async throws -> Self.TransformerDeprecated

associatedtype Transformer : TemporalTransformer

The transformer type created by this estimator.

**Required**

Deprecated

