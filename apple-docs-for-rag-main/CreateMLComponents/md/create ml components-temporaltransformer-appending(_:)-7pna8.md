

- Create ML Components
- TemporalTransformer
-  appending(\_:) 

Instance Method

# appending(\_:)

Composes this temporal transformer with another temporal transformer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func appending(_ other: Other) -> ComposedTemporalTransformer where Other : TemporalTransformer, Self.Output == Other.Input
```

## See Also

### Appending

func appending&lt;Other>(Other) -> ComposedTemporalTransformer&lt;Self, TransformerToTemporalAdaptor&lt;Other>>

Composes this temporal transformer with a transformer.

Deprecated

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

func appending&lt;Other>(Other) -> PreprocessingUpdatableTemporalEstimator&lt;Self, UpdatableEstimatorToTemporalAdaptor&lt;Other>>

Composes this temporal transformer with an updatable estimator.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingSupervisedTemporalEstimator&lt;Self, SupervisedEstimatorToTemporalAdaptor&lt;Other>>

Composes this transformer with a supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> PreprocessingUpdatableSupervisedTemporalEstimator&lt;Self, Other>

Composes this transformer with an updatable supervised temporal estimator.

Deprecated

