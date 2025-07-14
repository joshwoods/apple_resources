

- Create ML Components
- TabularTransformer
-  adaptedAsEstimator() 

Instance Method

# adaptedAsEstimator()

Exposes this tabular transformer as a trivial tabular estimator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func adaptedAsEstimator() -> TabularTransformerToEstimatorAdaptor
```

## See Also

### Applying and adapting

func appending&lt;Other>(Other) -> ComposedTabularTransformer&lt;Self, Other>

Composes this tabular transformer with another tabular transformer.

func adaptedAsUpdatableEstimator() -> TabularTransformerToUpdatableEstimatorAdaptor&lt;Self>

Exposes this tabular transformer as an updatable tabular estimator.

