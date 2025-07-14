

- Create ML Components
- UpdatableTabularEstimator
-  appending(\_:) 

Instance Method

# appending(\_:)

Composes this updatable tabular estimator with a tabular transformer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func appending(_ other: Other) -> some UpdatableTabularEstimator> where Other : TabularTransformer
```

## See Also

### Appending

func appending&lt;Other>(Other) -> some UpdatableTabularEstimator&lt;ComposedTabularTransformer&lt;Self.Transformer, Other.Transformer>> 

Composes this updatable tabular estimator with another updatable tabular estimator.

func appending&lt;Other>(Other) -> some UpdatableSupervisedTabularEstimator&lt;ComposedTabularTransformer&lt;Self.Transformer, Other.Transformer>, Other.Annotation> 

Composes this updatable tabular estimator with an updatable supervised tabular estimator.

