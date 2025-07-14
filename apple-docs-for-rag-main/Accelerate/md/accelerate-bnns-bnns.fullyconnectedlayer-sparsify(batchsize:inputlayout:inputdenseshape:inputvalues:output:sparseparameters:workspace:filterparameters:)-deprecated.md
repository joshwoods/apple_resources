

- Accelerate
- BNNS
- BNNS.FullyConnectedLayer
-  sparsify(batchSize:inputLayout:inputDenseShape:inputValues:output:sparseParameters:workspace:filterParameters:) Deprecated

Type Method

# sparsify(batchSize:inputLayout:inputDenseShape:inputValues:output:sparseParameters:workspace:filterParameters:)

Converts a sparse tensor from a standardized sparse layout to a device-specific sparse layout that Fully Connected uses.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
static func sparsify(
    batchSize: Int = 1,
    inputLayout layout: BNNS.SparseLayout,
    inputDenseShape: BNNSNDArrayDescriptor,
    inputValues: BNNSNDArrayDescriptor,
    output: inout BNNSNDArrayDescriptor,
    sparseParameters: BNNS.SparseParameters? = nil,
    workspace: UnsafeMutableRawBufferPointer? = nil,
    filterParameters: BNNSFilterParameters? = nil
) throws
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`batchSize`  

The number of input-output pairs to process.

`layout`  

The layout and nonzero indices of the sparse input.

`inputDenseShape`  

The dense shape of the sparse 2D input.

`inputValues`  

A 1D array descriptor that contains the nonzero input values.

`output`  

The destination array descriptor that contains the output-device-optimized BNNS Sparse Fully Connected weights.

`sparseParameters`  

An optional data structure that provides a hint to the sparsity function.

`workspace`  

An optional pointer to a memory region that the function uses as scratch space.

`filterParameters`  

The runtime filter parameters.

## See Also

### Sparse layers

func BNNSNDArrayGetDataSize(UnsafePointer&lt;BNNSNDArrayDescriptor>) -> Int

Returns the size, in bytes, that an array descriptor requires.

func BNNSNDArrayFullyConnectedSparsifySparseCOO(UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSSparsityParameters>?, Int, UnsafeMutableRawPointer?, Int, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Converts a sparse tensor from the standardized coordinate list (COO) layout to a device-specific sparse layout that BNNS fully connected layers use.

Deprecated

func BNNSNDArrayFullyConnectedSparsifySparseCSR(UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSSparsityParameters>?, Int, UnsafeMutableRawPointer?, Int, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Converts a sparse tensor from the standardized compressed sparse row (CSR) layout to a device-specific sparse layout that BNNS fully connected layers use.

Deprecated

struct SparseParameters

A data structure that provides a hint to the sparsity function.

Deprecated

enum SparseLayout

Constants that specify standardized sparse layouts that BNNS can convert to opaque.

Deprecated

enum SparsityType

Constants that specify patterns in the sparsity.

Deprecated

var BNNSSparsityTypeUnstructured: BNNSSparsityType

