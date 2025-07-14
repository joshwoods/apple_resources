

- Accelerate
-  BNNSGraphGetFunctionCount(\_:) 

Function

# BNNSGraphGetFunctionCount(\_:)

Returns the number of callable functions in the specified graph.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func BNNSGraphGetFunctionCount(_ graph: bnns_graph_t) -> Int
```

## Parameters 

`graph`  

The compiled graph object.

## Return Value

The number of callable functions in the specified graph, or `SIZE_T_MAX` if the query fails.

## See Also

### Querying a graph’s properties

func BNNSGraphGetArgumentIntents(bnns_graph_t, UnsafePointer&lt;CChar>?, Int, UnsafeMutablePointer&lt;BNNSGraphArgumentIntent>) -> Int32

Extracts the intents of arguments for the given function argument.

struct BNNSGraphArgumentIntent

Constants that describe argument intents.

func BNNSGraphGetArgumentCount(bnns_graph_t, UnsafePointer&lt;CChar>?) -> Int

Returns the number of arguments for the given function argument.

func BNNSGraphGetArgumentNames(bnns_graph_t, UnsafePointer&lt;CChar>?, Int, UnsafeMutablePointer&lt;UnsafePointer&lt;CChar>?>) -> Int32

Extracts the names of arguments for the given function argument.

func BNNSGraphGetFunctionNames(bnns_graph_t, Int, UnsafeMutablePointer&lt;UnsafePointer&lt;CChar>?>) -> Int32

Extracts the names of callable functions in the graph.

func BNNSGraphGetInputCount(bnns_graph_t, UnsafePointer&lt;CChar>?) -> Int

Returns the number of input arguments for the given function argument.

func BNNSGraphGetInputNames(bnns_graph_t, UnsafePointer&lt;CChar>?, Int, UnsafeMutablePointer&lt;UnsafePointer&lt;CChar>?>) -> Int32

Extracts the names of input arguments for the given function argument.

func BNNSGraphGetOutputCount(bnns_graph_t, UnsafePointer&lt;CChar>?) -> Int

Returns the number of output arguments for the given function argument.

func BNNSGraphGetOutputNames(bnns_graph_t, UnsafePointer&lt;CChar>?, Int, UnsafeMutablePointer&lt;UnsafePointer&lt;CChar>?>) -> Int32

Extracts the names of output arguments for the given function argument.

func BNNSGraphGetArgumentPosition(bnns_graph_t, UnsafePointer&lt;CChar>?, UnsafePointer&lt;CChar>) -> Int

Returns the index into the arguments array for the given function argument.

func BNNSGraphGetArgumentInterleaveFactors(bnns_graph_t, UnsafePointer&lt;CChar>?, Int, UnsafeMutablePointer&lt;UnsafePointer&lt;UInt16>?>, UnsafeMutablePointer&lt;Int>) -> Int32

Returns the interleave factors for arguments, if present

