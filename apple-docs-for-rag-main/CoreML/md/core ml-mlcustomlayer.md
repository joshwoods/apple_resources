

- Core ML
-  MLCustomLayer 

Protocol

# MLCustomLayer

An interface that defines the behavior of a custom layer in your neural network model.

iOS 11.2+iPadOS 11.2+Mac Catalyst 13.1+macOS 10.13.2+tvOS 11.2+visionOS 1.0+watchOS 4.2+

``` source
protocol MLCustomLayer
```

## Mentioned in 

Creating and Integrating a Model with Custom Layers

## Overview

You use the MLCustomLayer protocol to define the behavior of your own neural network layers in Core ML models. You can deploy novel or proprietary models on your own release schedule. Custom layers also provide a mechanism for pre- or post-processing during model evaluation.

## Topics

### Creating a Layer

init(parameters: [String : Any]) throws

Initializes the custom layer implementation.

**Required**

### Integrating a Layer

func setWeightData([Data]) throws

Assigns the weights for the connections within the layer.

**Required**

func outputShapes(forInputShapes: [[NSNumber]]) throws -> [[NSNumber]]

Calculates the shapes of the output of this layer for the given input shapes.

**Required**

### Evaluating a Layer

func evaluate(inputs: [MLMultiArray], outputs: [MLMultiArray]) throws

Evaluates the custom layer with the given inputs.

**Required**

func encode(commandBuffer: any MTLCommandBuffer, inputs: [any MTLTexture], outputs: [any MTLTexture]) throws

Encodes GPU commands to evaluate the custom layer.

## See Also

### Custom Model Layers

Creating and Integrating a Model with Custom Layers

Add models with custom neural-network layers to your app.

