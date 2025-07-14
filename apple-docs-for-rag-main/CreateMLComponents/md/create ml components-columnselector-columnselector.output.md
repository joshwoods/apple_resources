

- Create ML Components
- ColumnSelector
-  ColumnSelector.Output 

Type Alias

# ColumnSelector.Output

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
typealias Output = Estimator.Transformer.Output
```

## See Also

### Fitting a transformer

func fitted(to: DataFrame, eventHandler: EventHandler?) async throws -> ColumnSelector&lt;Estimator, UnwrappedInput>.Transformer

Fits a transformer to a data frame

typealias Input

typealias Transformer

The transformer type created by this estimator.

