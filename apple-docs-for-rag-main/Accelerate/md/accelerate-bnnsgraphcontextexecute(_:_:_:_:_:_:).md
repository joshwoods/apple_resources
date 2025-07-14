

- Accelerate
-  BNNSGraphContextExecute(\_:\_:\_:\_:\_:\_:) 

Function

# BNNSGraphContextExecute(\_:\_:\_:\_:\_:\_:)

Executes the specified function with the given context.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func BNNSGraphContextExecute(
    _ context: bnns_graph_context_t,
    _ function: UnsafePointer?,
    _ argument_count: Int,
    _ arguments: UnsafeMutablePointer,
    _ workspace_size: Int,
    _ workspace: UnsafeMutablePointer?
) -> Int32
```

## Parameters 

`context`  

The graph context. You may only use this context on a single thread at a time.

`function`  

The function. Specify as `nil` if the graph only contains one function.

`argument_count`  

The number of elements in the `arguments` array.

`arguments`  

An array of `bnns_graph_argument_t` objects that supply the input data and the outputs. Use the BNNSGraphGetArgumentPosition(_:_:_:) to derive the argument positions for this parameter. If you supply unallocated output arguments, this function allocates the required memory and reuses that memory for future executions.

`workspace_size`  

The size of the workspace. Call BNNSGraphContextGetWorkspaceSize(_:_:) to get the required size or pass `0` and a null `workspace` parameter to specify that this function allocates its own workspace.

`workspace`  

The temporary workspace that the function uses during execution. Call BNNSGraphContextGetWorkspaceSize(_:_:) to get the required size or pass `nil` and a zero `workspace_size` parameter to specify that this function allocates its own workspace.

## Return Value

`0` on success, nonzero on failure.

## Discussion

If the underlying model contains dynamic shaped inputs or outputs, you must set these prior to calling this routine with either BNNSGraphContextSetDynamicShapes(_:_:_:_:) or BNNSGraphContextSetBatchSize(_:_:_:). Don’t modify these shapes during execution.

This function doesn’t perform memory allocation if your code meets the following conditions:

- The workspace isn’t `nil`.

- The graph doesn’t contain tensors that BNNS couldn’t bound prior to calling this function.

- The arguments array doesn’t contain any new shape information.

- The code provides all output storage.

The following code executes the graph with the BNNSTensor structures `inputTensor` and `outputTensor` as the input and output arguments, respectively:

```
withUnsafeMutablePointer(to: &inputTensor) { input in
    withUnsafeMutablePointer(to: &outputTensor) { output in

        var inputArgument = bnns_graph_argument_t()
        inputArgument.tensor = input

        var outputArgument = bnns_graph_argument_t()
        outputArgument.tensor = output

        var arguments = [outputArgument, inputArgument]

        BNNSGraphContextSetArgumentType(context, BNNSGraphArgumentTypeTensor)

        BNNSGraphContextExecute(context, nil, 2, &arguments, 0, nil)
    }
}
```

## See Also

### Executing a graph

struct BNNSGraphArgumentType

Constants that specify the argument type for a graph context.

