

- Create ML Components
- TabularEstimator
-  fitted(to:eventHandler:) 

Instance Method

# fitted(to:eventHandler:)

Fits a transformer to a data frame

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func fitted(
    to input: DataFrame,
    eventHandler: EventHandler?
) async throws -> Self.Transformer
```

**Required**

## Parameters 

`input`  

A data frame containing examples.

`eventHandler`  

An event handler.

## Return Value

The fitted transformer.

## See Also

### Adapting and fitting

func adaptedAsSupervised&lt;Annotation>(annotationColumnID: ColumnID&lt;Annotation>) -> TabularEstimatorToSupervisedAdaptor&lt;Self, Annotation>

Exposes this tabular estimator as a supervised tabular estimator.

