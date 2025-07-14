

- Create ML Components
- UpdatableTabularEstimatorToSupervisedAdaptor
-  UpdatableTabularEstimatorToSupervisedAdaptor.Transformer 

Type Alias

# UpdatableTabularEstimatorToSupervisedAdaptor.Transformer

The transformer type created by this estimator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
typealias Transformer = Estimator.Transformer
```

## See Also

### Fitting

func fitted(to: DataFrame, validateOn: DataFrame?, eventHandler: EventHandler?) async throws -> UpdatableTabularEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Fits a transformer to a data frame.

func makeTransformer() -> Estimator.Transformer

Creates a default-initialized transformer suitable for incremental fitting.

func update(inout UpdatableTabularEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer, with: DataFrame, eventHandler: EventHandler?) async throws

Updates a transformer with a new data frame containing examples.

