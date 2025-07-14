

- Create ML Components
- TabularTransformer
-  appending(\_:) 

Instance Method

# appending(\_:)

Composes this tabular transformer with another tabular transformer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func appending(_ other: Other) -> ComposedTabularTransformer where Other : TabularTransformer
```

## See Also

### Applying and adapting

func adaptedAsEstimator() -> TabularTransformerToEstimatorAdaptor&lt;Self>

Exposes this tabular transformer as a trivial tabular estimator.

func adaptedAsUpdatableEstimator() -> TabularTransformerToUpdatableEstimatorAdaptor&lt;Self>

Exposes this tabular transformer as an updatable tabular estimator.

