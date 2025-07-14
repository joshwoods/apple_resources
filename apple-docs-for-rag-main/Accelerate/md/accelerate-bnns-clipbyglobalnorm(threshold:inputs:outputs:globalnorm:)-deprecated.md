

- Accelerate
- BNNS
-  clipByGlobalNorm(threshold:inputs:outputs:globalNorm:) Deprecated

Type Method

# clipByGlobalNorm(threshold:inputs:outputs:globalNorm:)

Clips the input tensors to a global Euclidean norm and writes the result to the output tensors.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+visionOSwatchOS 8.0+tvOS 15.0+

``` source
static func clipByGlobalNorm(
    threshold: Float,
    inputs: [BNNSNDArrayDescriptor],
    outputs: [BNNSNDArrayDescriptor],
    globalNorm: Float = 0
) throws
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`threshold`  

The maximum Euclidean norm to clip the gradient to.

`inputs`  

An array of input descriptors.

`outputs`  

An array of output descriptors.

`globalNorm`  

The global norm to use. Set to `0` to specify that the function computes the norm from the input descriptors.

## Discussion

Use this function to clip the values in an array of input tensors to a maximum global Euclidean norm. If you know the global norm of the input tensors, pass this value as the `globalNorm`. Otherwise, pass `0` to specify that the function calculates the norm.

The Euclidean norm is the square root of the sum of squares of the two tensors. The following code clips the Euclidean norm of two input tensors to half of the global Euclidean norm:

```
static func clipToGlobalNorm() {
    let inputOne = BNNSNDArrayDescriptor.allocate(
        initializingFrom: [1, 2, 3, 4] as [Float],
        shape: .vector(4))
    let inputTwo = BNNSNDArrayDescriptor.allocate(
        initializingFrom: [5, 6, 7, 8] as [Float],
        shape: .vector(4))

    let outputOne = BNNSNDArrayDescriptor.allocateUninitialized(
        scalarType: Float.self,
        shape: .vector(4))
    let outputTwo = BNNSNDArrayDescriptor.allocateUninitialized(
        scalarType: Float.self,
        shape: .vector(4))

    try? BNNS.clipByGlobalNorm(threshold: 0.5 * 14.2828568570857,
                               inputs: [inputOne, inputTwo],
                               outputs: [outputOne, outputTwo])

    // Prints: `[0.5, 1.0, 1.5, 2.0]`
    print(outputOne.makeArray(of: Float.self)!)

    // Prints: `[2.5, 3.0, 3.5, 4.0]`
    print(outputTwo.makeArray(of: Float.self)!)

    inputOne.deallocate()
    inputTwo.deallocate()
    outputOne.deallocate()
    outputTwo.deallocate()
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

