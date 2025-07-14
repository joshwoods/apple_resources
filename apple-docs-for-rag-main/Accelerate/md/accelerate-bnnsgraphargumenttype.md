

- Accelerate
-  BNNSGraphArgumentType 

Structure

# BNNSGraphArgumentType

Constants that specify the argument type for a graph context.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct BNNSGraphArgumentType
```

## Topics

### Argument types

init(UInt32)

Creates a new instance.

init(rawValue: UInt32)

Creates a new instance with the specified raw value.

### Instance Properties

var rawValue: UInt32

The corresponding value of the raw type.

var BNNSGraphArgumentTypePointer: BNNSGraphArgumentType

A pointer to the raw data for the tensor.

var BNNSGraphArgumentTypeTensor: BNNSGraphArgumentType

A tensor structure.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Specifying and querying a context’s properties

func BNNSGraphContextSetArgumentType(bnns_graph_context_t, BNNSGraphArgumentType) -> Int32

Specifies the argument type for a graph context.

func BNNSGraphContextSetDynamicShapes(bnns_graph_context_t, UnsafePointer&lt;CChar>?, Int, UnsafeMutablePointer&lt;bnns_graph_shape_t>) -> Int32

Specifies the dynamic shapes for a graph and, if possible, infers, the output shapes.

struct bnns_graph_shape_t

The specification of the shape of an argument.

func BNNSGraphContextSetBatchSize(bnns_graph_context_t, UnsafePointer&lt;CChar>?, UInt64) -> Int32

Sets the batch size for a graph.

func BNNSGraphContextEnableNanAndInfChecks(bnns_graph_context_t, Bool)

Specifies that the context checks intermediate tensors for NaNs and infinities.

func BNNSGraphContextGetWorkspaceSize(bnns_graph_context_t, UnsafePointer&lt;CChar>?) -> Int

Returns the minimum size, in bytes, of the workspace that graph context execution requires.

