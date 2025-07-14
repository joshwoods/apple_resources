

- Create ML Components
- ColumnSelector
-  decodeWithOptimizer(from:) 

Instance Method

# decodeWithOptimizer(from:)

Reads the encoded transformer and optimizer with a decoder.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func decodeWithOptimizer(from decoder: inout any EstimatorDecoder) throws -> ColumnSelector.Transformer
```

Available when `Estimator` conforms to `UpdatableEstimator` and `Estimator.Transformer.Input` is `UnwrappedInput?`.

## Parameters 

`decoder`  

A decoder.

## Return Value

The decoded transformer.

