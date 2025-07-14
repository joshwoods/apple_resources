

- Accelerate
- BNNSGraph
- BNNSGraph.Context
-  setBatchSize(\_:forFunction:) 

Instance Method

# setBatchSize(\_:forFunction:)

Sets the batch size for a graph.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOSwatchOS 11.0+

``` source
func setBatchSize(
    _ batchSize: Int,
    forFunction function: String? = nil
) async
```

## Parameters 

`batchSize`  

The batch size.

`function`  

The function. Specify as `nil` if the graph only contains one function.

## See Also

### Related Documentation

func BNNSGraphContextSetBatchSize(bnns_graph_context_t, UnsafePointer&lt;CChar>?, UInt64) -> Int32

Sets the batch size for a graph.

### Specifying and querying a graph context’s properties

func setDynamicShapes([BNNSGraph.Shape], forFunction: String?) async throws -> [BNNSGraph.Shape]

Specifies the dynamic shapes for a graph and, if possible, infers the output shapes.

struct Shape

The specification of the shape of an argument.

func argumentCount(forFunction: String?) -> Int

Returns the number of arguments for the given function argument.

func argumentNames(forFunction: String?) -> [String]

Returns the names of arguments for the given function argument.

func argumentPosition(forFunction: String?, argument: String) -> Int

Returns the index into the arguments array for the given function argument.

var functionCount: Int

The number of input arguments for the given function argument.

var functionNames: [String]

Returns the names of callable functions in the graph.

var checkForNaNsAndInfinities: Bool

A Boolean value that specifies that the context checks intermediate tensors for NaNs and infinities.

