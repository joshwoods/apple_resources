

- Create ML Components
- JointsSelector
-  appending(\_:) 

Instance Method

# appending(\_:)

Composes this transformer with an estimator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func appending(_ other: Other) -> PreprocessingEstimator where Other : Estimator, Self.Output == Other.Transformer.Input
```

