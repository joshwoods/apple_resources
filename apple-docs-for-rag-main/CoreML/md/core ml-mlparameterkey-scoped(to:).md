

- Core ML
- MLParameterKey
-  scoped(to:) 

Instance Method

# scoped(to:)

Creates a copy of a parameter key and adds the scope to it.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func scoped(to scope: String) -> MLParameterKey
```

## Parameters 

`scope`  

A scope that targets the key to an internal component of a model.

## Return Value

A new parameter key.

## Discussion

Use this method to target:

- A specific layer of a model

- A specific model within a pipeline model

- A specific layer of a model within a pipeline model

For example, to target an MLParameterKey to a layer in a model, scope the key with the layer’s name.

```
let weightsKey = MLParameterKey.weights

// Weights key scoped to the "FullyConnected" layer within a model.
let fullyConnectedWeights = weightsKey.scoped(to: "FullyConnected")

// Prints "Key 1: FullyConnected.weights".
print("Key 1: \(fullyConnectedWeights)")
```

To target a model within a pipeline model, scope the MLParameterKey with the model’s name.

```
// Number-of-neighbors key scoped to the first model in a pipeline model.
let firstModelNumberOfNeighbors = MLParameterKey.numberOfNeighbors.scoped(to: "model0")

// Prints "Key 2: model0.numberOfNeighbors".
print("Key 2: \(firstModelNumberOfNeighbors)")
```

To target a layer of a model within a pipeline model, start with an MLParameterKey you’ve already scoped to the model, and add an additional scope with the layer’s name.

```
let model1Biases = MLParameterKey.biases.scoped(to: "model1")

// Biases key scoped to the "FullyConnected" layer of the second model in a pipeline model.
let secondModelFullyConnectedBiases = model1Biases.scoped(to: "FullyConnected")

// Prints "Key 3: model1.FullyConnected.biases".
print("Key 3: \(secondModelFullyConnectedBiases)")
```

By default, a pipeline model names its individual models in the pipeline as `model0`, `model1`, and so on.

