

- Accelerate
- BNNS
- Classic BNNS API
-  Applying Filters 

API Collection

# Applying Filters

## Topics

### Forward Propagation Functions

func BNNSFilterApply(BNNSFilter?, UnsafeRawPointer, UnsafeMutableRawPointer) -> Int32

Applies a filter to an input, writing the result to a specified output.

Deprecated

func BNNSFilterApplyBatch(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeMutableRawPointer, Int) -> Int32

Applies a filter to a set of input objects, writing the result to a set of output objects.

Deprecated

func BNNSFilterApplyTwoInput(BNNSFilter?, UnsafeRawPointer, UnsafeRawPointer, UnsafeMutableRawPointer) -> Int32

Applies a filter to a pair of inputs, writing the result to a specified output.

Deprecated

func BNNSFilterApplyTwoInputBatch(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeRawPointer, Int, UnsafeMutableRawPointer, Int) -> Int32

Applies a filter to a set of input object pairs, writing the result to a set of output objects.

Deprecated

### Backpropagation Functions

func BNNSFilterApplyBackwardBatch(BNNSFilter?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeRawPointer?, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?) -> Int32

Applies a filter backward to generate input delta, weights delta and bias delta.

Deprecated

func BNNSFilterApplyBackwardTwoInputBatch(BNNSFilter?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeRawPointer?, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?) -> Int32

Applies a filter backward to generate input deltas, weights delta and bias delta.

Deprecated

## See Also

### General filters

typealias BNNSFilter

An opaque type that represents a filter.

Deprecated

class Layer

The base class for layer objects that wrap filters and manage deinitialization.

Deprecated

class UnaryLayer

The base class for layers that accept a single input.

Deprecated

class BinaryLayer

The base class for layers that accept two inputs.

Deprecated

struct BNNSFilterParameters

A structure that contains common filter parameters.

func BNNSFilterDestroy(BNNSFilter?)

Destroys the specified filter, releasing all resources allocated for it.

Deprecated

typealias BNNSAlloc

A type-alias for a user-provided memory allocation function.

typealias BNNSFree

A type-alias for a user-provided memory deallocation function.

