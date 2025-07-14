

- Create ML Components
- AnnotatedFeatureProvider
-  decodeWithOptimizer(from:) 

Instance Method

# decodeWithOptimizer(from:)

Reads the encoded transformer and optimizer with a decoder.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func decodeWithOptimizer(from decoder: inout any EstimatorDecoder) throws -> AnnotatedFeatureProvider.Transformer
```

Available when `Base` conforms to `UpdatableSupervisedEstimator` and `Base.Transformer.Input` is `UnwrappedInput?`.

## Parameters 

`decoder`  

A decoder.

## Return Value

The decoded transformer.

