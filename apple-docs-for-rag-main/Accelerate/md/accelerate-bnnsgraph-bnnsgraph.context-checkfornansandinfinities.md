

- Accelerate
- BNNSGraph
- BNNSGraph.Context
-  checkForNaNsAndInfinities 

Instance Property

# checkForNaNsAndInfinities

A Boolean value that specifies that the context checks intermediate tensors for NaNs and infinities.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOSwatchOS 11.0+

``` source
var checkForNaNsAndInfinities: Bool { get set }
```

## See Also

### Related Documentation

func BNNSGraphContextEnableNanAndInfChecks(bnns_graph_context_t, Bool)

Specifies that the context checks intermediate tensors for NaNs and infinities.

### Specifying and querying a graph context’s properties

func setBatchSize(Int, forFunction: String?) async

Sets the batch size for a graph.

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

