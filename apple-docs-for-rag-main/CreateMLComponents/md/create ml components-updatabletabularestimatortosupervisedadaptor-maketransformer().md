

- Create ML Components
- UpdatableTabularEstimatorToSupervisedAdaptor
-  makeTransformer() 

Instance Method

# makeTransformer()

Creates a default-initialized transformer suitable for incremental fitting.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func makeTransformer() -> Estimator.Transformer
```

## See Also

### Fitting

func fitted(to: DataFrame, validateOn: DataFrame?, eventHandler: EventHandler?) async throws -> UpdatableTabularEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer

Fits a transformer to a data frame.

func update(inout UpdatableTabularEstimatorToSupervisedAdaptor&lt;Estimator, Annotation>.Transformer, with: DataFrame, eventHandler: EventHandler?) async throws

Updates a transformer with a new data frame containing examples.

typealias Transformer

The transformer type created by this estimator.

