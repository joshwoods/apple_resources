

- Accelerate
- BNNS
-  clipByNorm(threshold:input:output:axes:) Deprecated

Type Method

# clipByNorm(threshold:input:output:axes:)

Clips the input tensor to a Euclidean norm and writes the result to the output tensor.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
static func clipByNorm(
    threshold: Float,
    input: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    axes: [Int]? = nil
) throws
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`threshold`  

The maximum Euclidean norm to clip the gradient to.

`input`  

The descriptor of the input.

`output`  

The descriptor of the output.

`axes`  

The dimensions that the function uses to compute the Euclidean norm. Set to `0` to specify that the function computes the norm over all dimensions.

## Discussion

Use this function to clip the values in an input tensor to a maximum Euclidean norm. The Euclidean norm is the square root of the sum of squares of the two tensors.

The function supports clipping across the entire tensor or by the norms of a dimension.

The following code clips the values on axis `1` to a Euclidean norm of `10`. The Euclidean norms of `[1, 2, 3]` and `[4, 5, 6]` are both less than `10` and function returns them unchanged. However, the Euclidean norm of `[7, 8, 9]` is greater than `10` and the function returns them scaled accordingly.

```
static func clipToNorm() {
    let inputValues: [Float] = [1, 2, 3,
                                4, 5, 6,
                                7, 8, 9]

    let input = BNNSNDArrayDescriptor.allocate(
        initializingFrom: inputValues,
        shape: .matrixRowMajor(3, 3))
    let output = BNNSNDArrayDescriptor.allocateUninitialized(
        scalarType: Float.self,
        shape: input.shape)

    try? BNNS.clipByNorm(threshold: 10,
                        input: input,
                        output: output,
                        axes: [1])

    // Prints `[1.0, 2.0, 3.0,
    //          4.0, 5.0, 6.0,
    //          5.0257072, 5.743665, 6.461623]`
    print(output.makeArray(of: Float.self)!)

    input.deallocate()
    output.deallocate()
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

static func clipByGlobalNorm(threshold: Float, inputs: [BNNSNDArrayDescriptor], outputs: [BNNSNDArrayDescriptor], globalNorm: Float) throws

Clips the input tensors to a global Euclidean norm and writes the result to the output tensors.

Deprecated

func BNNSClipByValue(UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, Float, Float) -> Int32

Clips a tensor’s values to the specified minimum and maximum values.

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

