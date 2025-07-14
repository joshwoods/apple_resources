

- Create ML Components
- UpdatableTemporalEstimatorToSupervisedAdaptor
-  UpdatableTemporalEstimatorToSupervisedAdaptor.Transformer Deprecated

Type Alias

# UpdatableTemporalEstimatorToSupervisedAdaptor.Transformer

The transformer type created by this estimator.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
typealias Transformer = Estimator.Transformer
```

## See Also

### Fitting and updating

func fitted&lt;InputSequence, FeatureSequence>(to: InputSequence, eventHandler: EventHandler?) async throws -> UpdatableTemporalEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Fits a transformer to a sequence of examples.

Deprecated

func fitted&lt;InputSequence, Validation, FeatureSequence>(to: InputSequence, validateOn: Validation, eventHandler: EventHandler?) async throws -> UpdatableTemporalEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Fits a transformer to a sequence of examples while validating with a validation sequence.

Deprecated

func makeTransformer() -> Estimator.Transformer

Creates a default-initialized transformer suitable for incremental fitting.

Deprecated

func update&lt;InputSequence, FeatureSequence>(inout UpdatableTemporalEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer, with: InputSequence, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of examples.

Deprecated

func update&lt;InputSequence, Validation, FeatureSequence>(inout UpdatableTemporalEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer, with: InputSequence, validateOn: Validation, eventHandler: EventHandler?) async throws

Fits a transformer to a sequence of examples while validating with a validation sequence.

Deprecated

