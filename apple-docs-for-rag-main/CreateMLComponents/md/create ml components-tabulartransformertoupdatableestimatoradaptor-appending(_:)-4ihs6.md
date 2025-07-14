

- Create ML Components
- TabularTransformerToUpdatableEstimatorAdaptor
-  appending(\_:) 

Instance Method

# appending(\_:)

Composes this updatable tabular estimator with an updatable supervised tabular estimator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func appending(_ other: Other) -> some UpdatableSupervisedTabularEstimator, Other.Annotation> where Other : UpdatableSupervisedTabularEstimator, Other.Annotation : Equatable
```

