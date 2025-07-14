

- Accelerate
- BNNS
-  applyActivation(activation:axes:input:output:batchSize:filterParameters:) Deprecated

Type Method

# applyActivation(activation:axes:input:output:batchSize:filterParameters:)

Applies an activation function on the specified axes.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+watchOS 8.0+visionOS

``` source
static func applyActivation(
    activation: BNNS.ActivationFunction,
    axes: [Int],
    input: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    batchSize: Int,
    filterParameters: BNNSFilterParameters? = nil
) throws
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`activation`  

The activation that the function applies.

`axes`  

The indices of the axes on which the function applies certain activation functions, such as softmax.

`input`  

The descriptor of the input.

`output`  

The descriptor of the output.

`batchSize`  

The number of input-output pairs.

`filterParameters`  

The filter runtime parameters.

## See Also

### Activation layers

func BNNSFilterCreateVectorActivationLayer(UnsafePointer&lt;BNNSVectorDescriptor>, UnsafePointer&lt;BNNSVectorDescriptor>, UnsafePointer&lt;BNNSActivation>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?Deprecated

class ActivationLayer

A layer object that wraps an activation filter and manages its deinitialization.

Deprecated

struct BNNSActivationFunction

Constants that describe activation functions.

struct BNNSActivation

A set of parameters that describe common activation functions.

struct BNNSLayerParametersActivation

A set of parameters that define an activation layer.

Deprecated

func BNNSFilterCreateLayerActivation(UnsafePointer&lt;BNNSLayerParametersActivation>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new activation layer.

Deprecated

func BNNSDirectApplyActivationBatch(UnsafePointer&lt;BNNSLayerParametersActivation>, UnsafePointer&lt;BNNSFilterParameters>?, Int, Int, Int) -> Int32

Applies an activation filter to a set of input objects, writing out the result to a set of output objects.

Deprecated

static func applyActivation(activation: BNNS.ActivationFunction, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, batchSize: Int, filterParameters: BNNSFilterParameters?) throws

Applies the specified activation function.

Deprecated

