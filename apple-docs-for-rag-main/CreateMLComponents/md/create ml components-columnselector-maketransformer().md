

- Create ML Components
- ColumnSelector
-  makeTransformer() 

Instance Method

# makeTransformer()

Creates a default-initialized transformer suitable for incremental fitting.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func makeTransformer() -> ColumnSelectorTransformer
```

Available when `Estimator` conforms to `UpdatableEstimator` and `Estimator.Transformer.Input` is `UnwrappedInput?`.

