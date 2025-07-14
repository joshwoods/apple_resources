

- Accelerate
-  BNNSGraphCompileFromFile(\_:\_:\_:) 

Function

# BNNSGraphCompileFromFile(\_:\_:\_:)

Compiles a source mlmodelc file to a graph object.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func BNNSGraphCompileFromFile(
    _ filename: UnsafePointer,
    _ function: UnsafePointer?,
    _ options: bnns_graph_compile_options_t
) -> bnns_graph_t
```

## Parameters 

`filename`  

The path to the source mlmodelc file.

`function`  

The name of the function that this operation compiles. Pass `nil` to specify that the operation compiles all the functions in the source file.

`options`  

The compilation options. Pass `nil` to specify that the operation uses the default set of options.

## Return Value

A compiled graph object. If the operation fails, the graph object’s data property is `nil`.

## Discussion

Xcode automatically compiles a Core ML model package (files with an `.mlpackage` file extension) into an mlmodelc file. The following code compiles a bnns_graph_t instance from a file named `myModel.mlpackage` that you copy into the project.

```
let options = BNNSGraphCompileOptionsMakeDefault()
defer {
    BNNSGraphCompileOptionsDestroy(options)
}

guard let fileName = Bundle.main.url(
    forResource: "myModel",
    withExtension: "mlmodelc")?.path() else {
    fatalError()
}

let graph = BNNSGraphCompileFromFile(fileName, 
                                     nil,
                                     options)

if graph.size == 0 {
    fatalError()
}
```

## See Also

### Related Documentation

Updating a Model File to a Model Package

Convert a Core ML model file into a model package in Xcode.

### Compiling a graph object

struct bnns_graph_t

The compiled graph object.

