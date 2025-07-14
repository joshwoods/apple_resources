

- Accelerate
- BNNSGraph
-  BNNSGraph.PointerArgument 

Protocol

# BNNSGraph.PointerArgument

A type that BNNS Graph accepts as an input-output argument.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOSwatchOS 11.0+

``` source
protocol PointerArgument
```

## Topics

### Querying a pointer argument’s properties

var baseAddress: UnsafeMutablePointer&lt;Self.Element>?

A pointer to the first element of the buffer.

**Required**

var count: Int

The number of elements in the buffer.

**Required**

### Associated Types

associatedtype Element

The pointer argument’s element type.

**Required**

## See Also

### Executing a graph

func executeFunction(String?, arguments: inout [BNNSTensor]) async throws

Executes the specified function using an array of input and output tensors.

func executeFunction&lt;T>(String?, arguments: [T]) throws

Executes the specified function using an array of input and output pointers.

