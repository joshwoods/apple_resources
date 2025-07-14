

- Create ML Components
- TabularEstimator
-  adaptedAsSupervised(annotationColumnID:) 

Instance Method

# adaptedAsSupervised(annotationColumnID:)

Exposes this tabular estimator as a supervised tabular estimator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func adaptedAsSupervised(annotationColumnID: ColumnID) -> TabularEstimatorToSupervisedAdaptor
```

## See Also

### Adapting and fitting

func fitted(to: DataFrame, eventHandler: EventHandler?) async throws -> Self.Transformer

Fits a transformer to a data frame

**Required**

