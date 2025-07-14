

- Create ML Components
- Estimator
-  fitted(to:) 

Instance Method

# fitted(to:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func fitted(to input: S) async throws -> Self.Transformer where S : Sequence, S.Element == Self.Transformer.Input
```

## See Also

### Fitting and adapting

func adaptedAsSupervised&lt;Annotation>(annotationType: Annotation.Type) -> EstimatorToSupervisedAdaptor&lt;Self, Annotation>

Exposes this estimator as a supervised estimator.

func adaptedAsTemporal() -> EstimatorToTemporalAdaptor&lt;Self>

Exposes this estimator as a temporal estimator.

Deprecated

func fitted&lt;S>(to: S, eventHandler: EventHandler?) async throws -> Self.Transformer

Fits a transformer to a sequence of examples.

**Required**

