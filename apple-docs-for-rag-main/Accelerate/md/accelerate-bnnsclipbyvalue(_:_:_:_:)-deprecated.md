

- Accelerate
-  BNNSClipByValue(\_:\_:\_:\_:) Deprecated

Function

# BNNSClipByValue(\_:\_:\_:\_:)

Clips a tensor’s values to the specified minimum and maximum values.

iOS 15.0–18.0DeprecatediPadOS 15.0–18.0DeprecatedMac Catalyst 15.0–18.0DeprecatedmacOS 12.0–15.0DeprecatedtvOS 15.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 8.0–11.0Deprecated

``` source
func BNNSClipByValue(
    _ dest: UnsafeMutablePointer,
    _ src: UnsafePointer,
    _ min_val: Float,
    _ max_val: Float
) -> Int32
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`dest`  

The descriptor of the output.

`src`  

The descriptor of the input.

`min_val`  

The minimum clipping value.

`max_val`  

The maximum clipping value.

## Discussion

Use this function to clip the values in an input tensor to the range you specify. The function sets values below the minimum to the minimum, and values above the maximum to the maximum.

The following code clips the values of the input tensor to the range `3...6`:

```
static func clipToBounds() {

    let inputData = UnsafeMutableBufferPointer.allocate(capacity: 8)
    _ = inputData.initialize(from: [1, 2, 3, 4, 5, 6, 7, 8])
    var inputDescriptor = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                                layout: BNNSDataLayoutVector,
                                                size: (8, 0, 0, 0, 0, 0, 0, 0),
                                                stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                                data: inputData.baseAddress!,
                                                data_type: BNNSDataType.float,
                                                table_data: nil,
                                                table_data_type: BNNSDataType.float,
                                                data_scale: 1, data_bias: 0)

    let outputData = UnsafeMutableBufferPointer.allocate(capacity: 8)
    var outputDescriptor = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                                 layout: BNNSDataLayoutVector,
                                                 size: (8, 0, 0, 0, 0, 0, 0, 0),
                                                 stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                                 data: outputData.baseAddress!,
                                                 data_type: BNNSDataType.float,
                                                 table_data: nil,
                                                 table_data_type: BNNSDataType.float,
                                                 data_scale: 1, data_bias: 0)

    BNNSClipByValue(&outputDescriptor,
                     &inputDescriptor,
                     3, 6)

    // Prints: `[3.0, 3.0, 3.0, 4.0, 5.0, 6.0, 6.0, 6.0]`
    print(Array(outputData))

    inputData.deallocate()
    outputData.deallocate()
}
```

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

func BNNSClipByNorm(UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, Float, UInt32) -> Int32

Clips a tensor’s values to a maximum Euclidean norm.

Deprecated

func BNNSClipByGlobalNorm(UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>>, UnsafeMutablePointer&lt;UnsafePointer&lt;BNNSNDArrayDescriptor>>, Int, Float, Float) -> Int32

Clips a tensor’s values to a maximum global Euclidean norm.

Deprecated

static func copyBandPart(BNNSNDArrayDescriptor, to: BNNSNDArrayDescriptor, lowerBandCount: Int?, upperBandCount: Int?, filterParameters: BNNSFilterParameters?) throws

Copies the specified subdiagonals and superdiagonals of a matrix, and sets other elements to zero.

Deprecated

