

- Create ML Components
- UpdatableEstimatorToTemporalAdaptor
-  UpdatableTemporalEstimator Implementations 

API Collection

# UpdatableTemporalEstimator Implementations

## Topics

### Instance Methods

func adaptedAsSupervised&lt;Annotation>(annotationType: Annotation.Type) -> UpdatableTemporalEstimatorToSupervisedAdaptor&lt;Self, Annotation>

Exposes this temporal estimator as a supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some UpdatableTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, TransformerToTemporalAdaptor&lt;Other.Transformer>>> 

Composes this updatable temporal estimator with an updatable estimator.

Deprecated

func appending&lt;Other>(Other) -> some UpdatableSupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, Other.Transformer>, Other.Annotation> 

Composes this updatable temporal estimator with an updatable supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some UpdatableSupervisedTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, TransformerToTemporalAdaptor&lt;Other.Transformer>>, Other.Annotation> 

Composes this updatable temporal estimator with an updatable supervised temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some UpdatableTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, Other.Transformer>> 

Composes this updatable temporal estimator with another updatable temporal estimator.

Deprecated

func appending&lt;Other>(Other) -> some UpdatableTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, TransformerToTemporalAdaptor&lt;Other>>> 

Composes this updatable temporal estimator with a transformer.

Deprecated

func appending&lt;Other>(Other) -> some UpdatableTemporalEstimator&lt;ComposedTemporalTransformer&lt;Self.Transformer, Other>> 

Composes this updatable temporal estimator with a temporal transformer.

Deprecated

func update&lt;InputSequence>(inout Self.Transformer, with: InputSequence) async throwsDeprecated

