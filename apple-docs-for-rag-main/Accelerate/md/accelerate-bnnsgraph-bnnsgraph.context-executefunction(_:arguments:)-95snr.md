

- Accelerate
- BNNSGraph
- BNNSGraph.Context
-  executeFunction(\_:arguments:) 

Instance Method

# executeFunction(\_:arguments:)

Executes the specified function using an array of input and output pointers.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOSwatchOS 11.0+

``` source
func executeFunction(
    _ function: String? = nil,
    arguments: [T]
) throws where T : BNNSGraph.PointerArgument
```

## Parameters 

`function`  

The function. Specify as `nil` if the graph only contains one function.

`arguments`  

The output and input arguments. Note that the arguments may not be in the same order as the original `mlpackage` or `mlmodelc` file. Use the argumentPosition(forFunction:argument:) function to get the correct position in the `arguments` array for a given argument.

## See Also

### Executing a graph

func executeFunction(String?, arguments: inout [BNNSTensor]) async throws

Executes the specified function using an array of input and output tensors.

protocol PointerArgument

A type that BNNS Graph accepts as an input-output argument.

