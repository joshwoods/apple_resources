

- Create ML Components
- Estimator
-  adaptedAsSupervised(annotationType:) 

Instance Method

# adaptedAsSupervised(annotationType:)

Exposes this estimator as a supervised estimator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func adaptedAsSupervised(annotationType: Annotation.Type = Annotation.self) -> EstimatorToSupervisedAdaptor where Annotation : Equatable
```

## See Also

### Fitting and adapting

func adaptedAsTemporal() -> EstimatorToTemporalAdaptor&lt;Self>

Exposes this estimator as a temporal estimator.

Deprecated

func fitted&lt;S>(to: S, eventHandler: EventHandler?) async throws -> Self.Transformer

Fits a transformer to a sequence of examples.

**Required**

func fitted&lt;S>(to: S) async throws -> Self.Transformer

