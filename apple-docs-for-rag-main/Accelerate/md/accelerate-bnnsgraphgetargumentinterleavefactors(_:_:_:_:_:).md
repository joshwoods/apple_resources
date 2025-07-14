

- Accelerate
-  BNNSGraphGetArgumentInterleaveFactors(\_:\_:\_:\_:\_:) 

Function

# BNNSGraphGetArgumentInterleaveFactors(\_:\_:\_:\_:\_:)

Returns the interleave factors for arguments, if present

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func BNNSGraphGetArgumentInterleaveFactors(
    _ graph: bnns_graph_t,
    _ function: UnsafePointer?,
    _ argument_count: Int,
    _ argument_interleave: UnsafeMutablePointer?>,
    _ argument_interleave_counts: UnsafeMutablePointer
) -> Int32
```

## Discussion

If any arguments to the function are specified with an interleave factor (e.g. using the `interleave` option to `tensor_buffer` in MIL), this function can be used to retrieve the interleave factor array.

Arguments:

- `graph`: object to query.

- `function`: function to query. It may be `NULL` if there is only one function.

- `argument_count`: number of elements in `argument_interleave` and in `argument_interleave_counts`.

- `argument_interleave`: array of pointers to interleave factors to populate. On exit `argument_interleave[i]` will be set to either:

  - `NULL` if argument `i` has no interleave factor; or

  - a pointer into the graph object containing the interleave factors that contains `argument_interleave_counts[i]` elements. Only the first \[0, min(argument_count, argument_interleave)) entries are set.

- `argument_interleave_counts`: gives the size of the array pointed to by `argument_interleave[i]`, or is set to 0 if `argument_interleave[i]` is set to `NULL`.

Returns: 0 on success, nonzero on failure. Failure may be caused by either invalid values of `graph` or `function`.

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

