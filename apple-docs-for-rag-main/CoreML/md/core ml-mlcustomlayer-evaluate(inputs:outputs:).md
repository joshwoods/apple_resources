

- Core ML
- MLCustomLayer
-  evaluate(inputs:outputs:) 

Instance Method

# evaluate(inputs:outputs:)

Evaluates the custom layer with the given inputs.

iOS 11.2+iPadOS 11.2+Mac Catalyst 13.1+macOS 10.13.2+tvOS 11.2+visionOS 1.0+watchOS 4.2+

``` source
func evaluate(
    inputs: [MLMultiArray],
    outputs: [MLMultiArray]
) throws
```

**Required**

## Parameters 

`inputs`  

The array of inputs to be evaluated.

`outputs`  

The array of outputs to be populated by evaluating the given inputs.

## Mentioned in 

Creating and Integrating a Model with Custom Layers

## Discussion

Implement this method to evaluate the inputs using your layer’s custom behavior and to populate the output arrays. It will be called for each evaluation of your model performed on the CPU.

The memory for both input and output arrays is preallocated; don’t copy or move it. The inputs and outputs will have the shapes of the most recent call to outputShapes(forInputShapes:). Don’t modify the input values.

Investigate vecLib for methods that could optimize your implementation significantly.

## See Also

### Evaluating a Layer

func encode(commandBuffer: any MTLCommandBuffer, inputs: [any MTLTexture], outputs: [any MTLTexture]) throws

Encodes GPU commands to evaluate the custom layer.

