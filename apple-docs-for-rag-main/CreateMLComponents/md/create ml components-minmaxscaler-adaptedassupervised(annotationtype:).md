

- Create ML Components
- MinMaxScaler
-  adaptedAsSupervised(annotationType:) 

Instance Method

# adaptedAsSupervised(annotationType:)

Exposes this estimator as a supervised estimator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func adaptedAsSupervised(annotationType: Annotation.Type = Annotation.self) -> EstimatorToSupervisedAdaptor where Annotation : Equatable
```

