

- Accelerate
-  BNNSClipByGlobalNorm(\_:\_:\_:\_:\_:) Deprecated

Function

# BNNSClipByGlobalNorm(\_:\_:\_:\_:\_:)

Clips a tensor’s values to a maximum global Euclidean norm.

iOS 15.0–18.0DeprecatediPadOS 15.0–18.0DeprecatedMac Catalyst 15.0–18.0DeprecatedmacOS 12.0–15.0DeprecatedtvOS 15.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 8.0–11.0Deprecated

``` source
func BNNSClipByGlobalNorm(
    _ dest: UnsafeMutablePointer>,
    _ src: UnsafeMutablePointer>,
    _ count: Int,
    _ max_norm: Float,
    _ use_norm: Float
) -> Int32
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`dest`  

An array of output descriptors.

`src`  

An array of input descriptors.

`count`  

The number of input and output descriptors.

`max_norm`  

The maximum global Euclidean norm.

`use_norm`  

An optional value for a known global Euclidean norm. Set to `0` to specify that the function computes the norm from the input descriptors.

## Discussion

Use this function to clip the values in an array of input tensors to a maximum Euclidean norm. If you know the global norm of the input tensors, pass this value as the `use_norm`. Otherwise, pass `0` to specify that the function calculates the norm.

The Euclidean norm is the square root of the sum of squares of the two tensors. The following code clips the Euclidean norm of two input tensors to half of the global Euclidean norm:

```
static func clipToGlobalNorm() {

    let inputOneData = UnsafeMutableBufferPointer.allocate(capacity: 4)
    _ = inputOneData.initialize(from: [1, 2, 3, 4])
    let inputOneDescriptor = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                                   layout: BNNSDataLayoutVector,
                                                   size: (4, 0, 0, 0, 0, 0, 0, 0),
                                                   stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                                   data: inputOneData.baseAddress!,
                                                   data_type: BNNSDataType.float,
                                                   table_data: nil,
                                                   table_data_type: BNNSDataType.float,
                                                   data_scale: 1, data_bias: 0)

    let inputTwoData = UnsafeMutableBufferPointer.allocate(capacity: 4)
    _ = inputTwoData.initialize(from: [5, 6, 7, 8])
    let inputTwoDescriptor = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                                   layout: BNNSDataLayoutVector,
                                                   size: (4, 0, 0, 0, 0, 0, 0, 0),
                                                   stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                                   data: inputTwoData.baseAddress!,
                                                   data_type: BNNSDataType.float,
                                                   table_data: nil,
                                                   table_data_type: BNNSDataType.float,
                                                   data_scale: 1, data_bias: 0)

    let outputOneData = UnsafeMutableBufferPointer.allocate(capacity: 4)
    let outputOneDescriptor = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                                    layout: BNNSDataLayoutVector,
                                                    size: (4, 0, 0, 0, 0, 0, 0, 0),
                                                    stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                                    data: outputOneData.baseAddress!,
                                                    data_type: BNNSDataType.float,
                                                    table_data: nil,
                                                    table_data_type: BNNSDataType.float,
                                                    data_scale: 1, data_bias: 0)

    let outputTwoData = UnsafeMutableBufferPointer.allocate(capacity: 4)
    let outputTwoDescriptor = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                                    layout: BNNSDataLayoutVector,
                                                    size: (4, 0, 0, 0, 0, 0, 0, 0),
                                                    stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                                    data: outputTwoData.baseAddress!,
                                                    data_type: BNNSDataType.float,
                                                    table_data: nil,
                                                    table_data_type: BNNSDataType.float,
                                                    data_scale: 1, data_bias: 0)

    let inputs = [inputOneDescriptor, inputTwoDescriptor]
    var inputsPointers: [UnsafePointer] = inputs.map { input in
        var descriptor = input

        let inputPtr = UnsafeMutablePointer.allocate(capacity: 1)
        inputPtr.initialize(from: &descriptor, count: 1)

        return UnsafePointer(inputPtr)
    }

    let outputs = [outputOneDescriptor, outputTwoDescriptor]
    var outputsPointers: [UnsafeMutablePointer] = outputs.map { output in
        var descriptor = output

        let outputPtr = UnsafeMutablePointer.allocate(capacity: 1)
        outputPtr.initialize(from: &descriptor, count: 1)

        return outputPtr
    }

    BNNSClipByGlobalNorm(&outputsPointers,
                         &inputsPointers,
                         2,
                         0.5 * 14.2828568570857,
                         0)

    // Prints: `[0.5, 1.0, 1.5, 2.0]`
    print(Array(outputOneData))

    // Prints: `[2.5, 3.0, 3.5, 4.0]`
    print(Array(outputTwoData))

    inputOneData.deallocate()
    inputTwoData.deallocate()
    outputOneData.deallocate()
    outputTwoData.deallocate()
}
```

On return, `outputOne` contains the values `[0.5, 1.0, 1.5, 2.0]`, and `outputTwo` contains the values `[2.5, 3.0, 3.5, 4.0]`.

## See Also

### Utility functions

static func copy(BNNSNDArrayDescriptor, to: BNNSNDArrayDescriptor, filterParameters: BNNSFilterParameters?) throws

Copies the contents of an n-dimensional array descriptor to another descriptor of the same shape.

static func transpose(input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, firstTransposeAxis: Int, secondTransposeAxis: Int, filterParameters: BNNSFilterParameters?) throws

Transposes a tensor by swapping two of its dimensions.

func BNNSCopy(UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Copies the contents of an n-dimensional array descriptor to another of the same shape.

func BNNSTranspose(UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, Int, Int, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Transposes a tensor by swapping two of its dimensions.

func BNNSGetPointer(BNNSFilter?, BNNSPointerSpecifier) -> BNNSNDArrayDescriptor

Returns an n-dimensional array descriptor that contains a reference to a filter-data member.

Deprecated

struct BNNSPointerSpecifier

Constants that specify which pointer the BNNS get filter function returns.

class GramLayer

A layer object that wraps a Gram matrix filter and manages its deinitialization.

Deprecated

struct BNNSLayerParametersGram

A set of parameters that define a Gram matrix layer.

Deprecated

func BNNSFilterCreateLayerGram(UnsafePointer&lt;BNNSLayerParametersGram>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new Gram matrix layer.

Deprecated

static func clip(to: ClosedRange&lt;Float>, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor) throws

Clips the input tensor to a closed range and writes the result to the output tensor.

Deprecated

static func clipByNorm(threshold: Float, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axes: [Int]?) throws

Clips the input tensor to a Euclidean norm and writes the result to the output tensor.

Deprecated

static func clipByGlobalNorm(threshold: Float, inputs: [BNNSNDArrayDescriptor], outputs: [BNNSNDArrayDescriptor], globalNorm: Float) throws

Clips the input tensors to a global Euclidean norm and writes the result to the output tensors.

Deprecated

func BNNSClipByValue(UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, Float, Float) -> Int32

Clips a tensor’s values to the specified minimum and maximum values.

Deprecated

func BNNSClipByNorm(UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, Float, UInt32) -> Int32

Clips a tensor’s values to a maximum Euclidean norm.

Deprecated

static func copyBandPart(BNNSNDArrayDescriptor, to: BNNSNDArrayDescriptor, lowerBandCount: Int?, upperBandCount: Int?, filterParameters: BNNSFilterParameters?) throws

Copies the specified subdiagonals and superdiagonals of a matrix, and sets other elements to zero.

Deprecated

