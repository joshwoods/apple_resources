

- Create ML Components
- UpdatableSupervisedTabularEstimator
-  appending(\_:) 

Instance Method

# appending(\_:)

Composes this supervised tabular estimator with an updatable tabular estimator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func appending(_ other: Other) -> some UpdatableSupervisedTabularEstimator, Self.Annotation> where Other : UpdatableTabularEstimator, Self.Annotation : Equatable
```

## See Also

### Appending

func appending&lt;Other>(Other) -> some UpdatableSupervisedTabularEstimator&lt;ComposedTabularTransformer&lt;Self.Transformer, Other.Transformer>, Self.Annotation> 

Composes this supervised tabular estimator with another supervised tabular estimator.

func appending&lt;Other>(Other) -> some UpdatableSupervisedTabularEstimator&lt;ComposedTabularTransformer&lt;Self.Transformer, Other>, Self.Annotation> 

Composes this supervised tabular estimator with a tabular transformer.

