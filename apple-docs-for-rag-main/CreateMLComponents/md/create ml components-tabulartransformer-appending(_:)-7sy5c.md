

- Create ML Components
- TabularTransformer
-  appending(\_:) 

Instance Method

# appending(\_:)

Composes this transformer with a supervised tabular estimator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func appending(_ other: Other) -> some SupervisedTabularEstimator, Other.Annotation> where Other : SupervisedTabularEstimator
```

## See Also

### Appending

func appending&lt;Other>(Other) -> PreprocessingSupervisedTabularEstimator&lt;Self, Other>

Composes this transformer with a supervised tabular estimator.

func appending&lt;Other>(Other) -> PreprocessingUpdatableTabularEstimator&lt;Self, Other>

Composes this transformer with an updatable estimator.

func appending&lt;Other>(Other) -> PreprocessingTabularEstimator&lt;Self, Other>

Composes this transformer with an estimator.

func appending&lt;Other>(Other) -> PreprocessingUpdatableSupervisedTabularEstimator&lt;Self, Other>

Composes this transformer with an updatable supervised estimator.

func appending&lt;Other>(Other) -> some TabularEstimator&lt;ComposedTabularTransformer&lt;Self, Other.Transformer>> 

Compose this tabular transformer with a tabular estimator.

