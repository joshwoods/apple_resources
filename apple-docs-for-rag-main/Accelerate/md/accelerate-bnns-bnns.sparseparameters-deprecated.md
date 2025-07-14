

- Accelerate
- BNNS
-  BNNS.SparseParameters Deprecated

Structure

# BNNS.SparseParameters

A data structure that provides a hint to the sparsity function.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
struct SparseParameters
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Creating a Sparse Parameters Structure

init(type: BNNS.SparsityType, ratio: (numerator: UInt32, denominator: UInt32), targetSystem: BNNSTargetSystem)

Returns a new sparse parameters structure.

### Inspecting the Properties of a Sparse Parameters Structure

let ratio: (numerator: UInt32, denominator: UInt32)

The sparsity ratio expressed as the numerator and the denominator.

let targetSystem: BNNSTargetSystem

The target system.

let type: BNNS.SparsityType

An enumeration that specifies special patterns, if any, in the sparsity.

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

static func sparsify(batchSize: Int, inputLayout: BNNS.SparseLayout, inputDenseShape: BNNSNDArrayDescriptor, inputValues: BNNSNDArrayDescriptor, output: inout BNNSNDArrayDescriptor, sparseParameters: BNNS.SparseParameters?, workspace: UnsafeMutableRawBufferPointer?, filterParameters: BNNSFilterParameters?) throws

Converts a sparse tensor from a standardized sparse layout to a device-specific sparse layout that Fully Connected uses.

Deprecated

enum SparseLayout

Constants that specify standardized sparse layouts that BNNS can convert to opaque.

Deprecated

enum SparsityType

Constants that specify patterns in the sparsity.

Deprecated

var BNNSSparsityTypeUnstructured: BNNSSparsityType

