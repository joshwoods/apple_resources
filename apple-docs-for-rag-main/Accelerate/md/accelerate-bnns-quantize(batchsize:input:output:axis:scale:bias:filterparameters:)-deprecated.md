

- Accelerate
- BNNS
-  quantize(batchSize:input:output:axis:scale:bias:filterParameters:) Deprecated

Type Method

# quantize(batchSize:input:output:axis:scale:bias:filterParameters:)

Quantizes the input tensor and writes the result to the output tensor.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+Mac Catalyst

``` source
static func quantize(
    batchSize: Int,
    input: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    axis: Int? = nil,
    scale: BNNSNDArrayDescriptor?,
    bias: BNNSNDArrayDescriptor?,
    filterParameters: BNNSFilterParameters? = nil
) throws
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`batchSize`  

The number of input-output pairs to process.

`input`  

The descriptor of the input.

`output`  

The descriptor of the output.

`axis`  

The index of the axis to which the function applies scale and bias. Set to `nil` to dequantize the entire tensor using scale and bias.

`scale`  

The scale, set to `nil` for a scale of `1.0`.

`bias`  

The bias, set to `nil` for a bias of `0.0`.

`filterParameters`  

Runtime filter parameters.

## Discussion

The following code quantizes a single-precision matrix to a 16-bit integer matrix. The code applies the scale along the zeroth axis and, therefore, the scale tensor contains four elements.

```
static func quantize() {

    let inputValues = [1, 2, 3, 4,
                       5, 6, 7, 8] as [Float]

    let input = BNNSNDArrayDescriptor.allocate(
        initializingFrom: inputValues,
        shape: .matrixRowMajor(4, 2))

    let output = BNNSNDArrayDescriptor.allocateUninitialized(
        scalarType: Int16.self,
        shape: input.shape)

    let scale = BNNSNDArrayDescriptor.allocate(
        initializingFrom: [1, 10, 100, 1000] as [Float],
        shape: .vector(4))

    try? BNNS.quantize(batchSize: 1,
                       input: input,
                       output: output,
                       axis: 0,
                       scale: scale,
                       bias: nil)

    // Prints:
    //  [1, 20, 300, 4000,
    //   5, 60, 700, 8000]
    print(output.makeArray(of: Int16.self)!)

    input.deallocate()
    output.deallocate()
    scale.deallocate()
}
```

## See Also

### Related Documentation

var BNNSQuantizerFunctionQuantize: BNNSQuantizerFunction

A constant that specifes conversion to a lower precision.

### Quantization functions

static func dequantize(batchSize: Int, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axis: Int?, scale: BNNSNDArrayDescriptor?, bias: BNNSNDArrayDescriptor?, filterParameters: BNNSFilterParameters?) throws

Dequantizes the input tensor and writes the result to the output tensor.

Deprecated

struct BNNSQuantizerFunction

Constants that describe quantization functions.

struct BNNSLayerParametersQuantization

A structure that contains the parameters of a quantization layer.

Deprecated

func BNNSDirectApplyQuantizer(UnsafePointer&lt;BNNSLayerParametersQuantization>, UnsafePointer&lt;BNNSFilterParameters>?, Int, Int, Int) -> Int32

Applies a quantization layer directly to two input matrices.

Deprecated

