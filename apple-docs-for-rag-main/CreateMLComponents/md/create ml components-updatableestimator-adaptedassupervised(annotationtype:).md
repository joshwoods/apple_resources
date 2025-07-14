

- Create ML Components
- UpdatableEstimator
-  adaptedAsSupervised(annotationType:) 

Instance Method

# adaptedAsSupervised(annotationType:)

Exposes this estimator as a supervised estimator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func adaptedAsSupervised(annotationType: Annotation.Type = Annotation.self) -> UpdatableEstimatorToSupervisedAdaptor where Annotation : Equatable
```

## See Also

### Adapting

func adaptedAsTemporal() -> UpdatableEstimatorToTemporalAdaptor&lt;Self>

Exposes this estimator as a temporal estimator.

Deprecated

