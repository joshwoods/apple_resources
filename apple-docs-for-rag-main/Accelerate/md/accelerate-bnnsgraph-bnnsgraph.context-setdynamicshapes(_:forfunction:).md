

- Accelerate
- BNNSGraph
- BNNSGraph.Context
-  setDynamicShapes(\_:forFunction:) 

Instance Method

# setDynamicShapes(\_:forFunction:)

Specifies the dynamic shapes for a graph and, if possible, infers the output shapes.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOSwatchOS 11.0+

``` source
func setDynamicShapes(
    _ shapes: [BNNSGraph.Shape],
    forFunction function: String? = nil
) async throws -> [BNNSGraph.Shape]
```

## Parameters 

`shapes`  

An array of input shapes in the same order as you pass to BNNSGraphContextExecute(_:_:_:_:_:_:).

This function reads input shapes with a nonzero rank, and uses the constant or default value from the source model for input shapes with a zero rank. The function generates an error for shapes with a nonzero value that doesn’t match the source model.

`function`  

The function. Specify as `nil` if the graph only contains one function.

## See Also

### Related Documentation

func BNNSGraphContextSetDynamicShapes(bnns_graph_context_t, UnsafePointer&lt;CChar>?, Int, UnsafeMutablePointer&lt;bnns_graph_shape_t>) -> Int32

Specifies the dynamic shapes for a graph and, if possible, infers, the output shapes.

### Specifying and querying a graph context’s properties

func setBatchSize(Int, forFunction: String?) async

Sets the batch size for a graph.

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

