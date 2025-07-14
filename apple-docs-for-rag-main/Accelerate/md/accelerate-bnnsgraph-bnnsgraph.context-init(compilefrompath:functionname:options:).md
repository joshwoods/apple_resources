

- Accelerate
- BNNSGraph
- BNNSGraph.Context
-  init(compileFromPath:functionName:options:) 

Initializer

# init(compileFromPath:functionName:options:)

Returns a new context that wraps a graph object representing the compiled mlmodelc file.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOSwatchOS 11.0+

``` source
init(
    compileFromPath path: String,
    functionName: String? = nil,
    options: BNNSGraph.CompileOptions = CompileOptions()
) async throws
```

## Parameters 

`path`  

The path to the source mlmodelc file.

`functionName`  

The name of the function that this operation compiles. Pass `nil` to specify that the operation compiles all the functions in the source file.

`options`  

The compilation options.

## See Also

### Related Documentation

func BNNSGraphCompileFromFile(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>?, bnns_graph_compile_options_t) -> bnns_graph_t

Compiles a source mlmodelc file to a graph object.

func BNNSGraphContextMake(bnns_graph_t) -> bnns_graph_context_t

Returns an allocated and initialized graph context from the specified graph.

### Creating a graph context

struct CompileOptions

The compilation options that BNNS uses when compiling a source mlmodelc file to a graph object.

