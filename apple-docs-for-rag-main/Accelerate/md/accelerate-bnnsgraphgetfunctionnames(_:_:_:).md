

- Accelerate
-  BNNSGraphGetFunctionNames(\_:\_:\_:) 

Function

# BNNSGraphGetFunctionNames(\_:\_:\_:)

Extracts the names of callable functions in the graph.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func BNNSGraphGetFunctionNames(
    _ graph: bnns_graph_t,
    _ function_name_count: Int,
    _ function_names: UnsafeMutablePointer?>
) -> Int32
```

## Parameters 

`graph`  

The compiled graph object.

`function_name_count`  

The number of elements in the `function_names` array.

`function_names`  

On output, an array of pointers to strings that contain the function names.

## Return Value

`0` on success, nonzero on failure.

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

func BNNSGraphGetFunctionCount(bnns_graph_t) -> Int

Returns the number of callable functions in the specified graph.

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

