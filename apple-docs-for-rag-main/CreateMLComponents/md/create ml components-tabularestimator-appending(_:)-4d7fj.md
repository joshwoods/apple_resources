

- Create ML Components
- TabularEstimator
-  appending(\_:) 

Instance Method

# appending(\_:)

Compose this tabular estimator with a tabular transformer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func appending(_ other: Other) -> some TabularEstimator> where Other : TabularTransformer
```

## See Also

### Appending

func appending&lt;Other>(Other) -> some TabularEstimator&lt;ComposedTabularTransformer&lt;Self.Transformer, Other.Transformer>> 

Compose this tabular estimator with another tabular estimator.

func appending&lt;Other>(Other) -> some SupervisedTabularEstimator&lt;ComposedTabularTransformer&lt;Self.Transformer, Other.Transformer>, Other.Annotation> 

Composes this tabular estimator with a supervised tabular estimator.

