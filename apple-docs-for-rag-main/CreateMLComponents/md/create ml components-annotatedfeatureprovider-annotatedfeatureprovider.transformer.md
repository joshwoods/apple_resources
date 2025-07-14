

- Create ML Components
- AnnotatedFeatureProvider
-  AnnotatedFeatureProvider.Transformer 

Type Alias

# AnnotatedFeatureProvider.Transformer

The transformer type created by this estimator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
typealias Transformer = ColumnSelectorTransformer
```

## See Also

### Fitting

func fitted(to: DataFrame, validateOn: DataFrame?, eventHandler: EventHandler?) async throws -> ColumnSelectorTransformer&lt;Base.Transformer, UnwrappedInput>

Fits a transformer to a data frame

