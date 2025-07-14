

- Core ML
- MLCustomLayer
-  outputShapes(forInputShapes:) 

Instance Method

# outputShapes(forInputShapes:)

Calculates the shapes of the output of this layer for the given input shapes.

iOS 11.2+iPadOS 11.2+Mac Catalyst 13.1+macOS 10.13.2+tvOS 11.2+visionOS 1.0+watchOS 4.2+

``` source
func outputShapes(forInputShapes inputShapes: [[NSNumber]]) throws -> [[NSNumber]]
```

**Required**

## Parameters 

`inputShapes`  

The shapes of the input for this layer.

## Return Value

The shapes of the output for the given input shapes.

## Mentioned in 

Creating and Integrating a Model with Custom Layers

## Discussion

Implement this method to define the layer’s interface with the rest of the network. It will be called at least once at load time and any time the size of the inputs changes in a call to prediction(from:).

This method consumes and returns arrays of shapes, for inputs and outputs of the custom layer, respectively. See the Core ML Neural Network specification for more details about shapes and how layers use them.

## See Also

### Integrating a Layer

func setWeightData([Data]) throws

Assigns the weights for the connections within the layer.

**Required**

