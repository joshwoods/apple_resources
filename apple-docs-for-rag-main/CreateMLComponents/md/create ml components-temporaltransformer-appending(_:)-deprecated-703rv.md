

- Create ML Components
- TemporalTransformer
-  appending(\_:) Deprecated

Instance Method

# appending(\_:)

Composes this temporal transformer with an updatable estimator.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func appending(_ other: Other) -> PreprocessingUpdatableTemporalEstimator> where Other : UpdatableEstimator, Self.Output == Other.Transformer.Input
```

## See Also

### Appending

func appending&lt;Other>(Other) -> ComposedTemporalTransformer&lt;Self, TransformerToTemporalAdaptor&lt;Other>>

Composes this temporal transformer with a transformer.

Deprecated

func appending&lt;Other>(Other) -> ComposedTemporalTransformer&lt;Self, Other>

Composes this temporal transformer with another temporal transformer.

func appending&lt;Other>(Other) -> PreprocessingSupervisedTemporalEstimator&lt;Self, Other>

Composes this transformer with a supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingUpdatableTemporalEstimator&lt;Self, Other>

Composes this temporal transformer with an updatable temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingUpdatableSupervisedTemporalEstimator&lt;Self, UpdatableSupervisedEstimatorToTemporalAdaptor&lt;Other>>

Composes this transformer with an updatable supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingTemporalEstimator&lt;Self, Other>

Composes this temporal transformer with a temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingTemporalEstimator&lt;Self, EstimatorToTemporalAdaptor&lt;Other>>

Composes this temporal transformer with an estimator.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingSupervisedTemporalEstimator&lt;Self, SupervisedEstimatorToTemporalAdaptor&lt;Other>>

Composes this transformer with a supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingUpdatableSupervisedTemporalEstimator&lt;Self, Other>

Composes this transformer with an updatable supervised temporal estimator.

Deprecated

