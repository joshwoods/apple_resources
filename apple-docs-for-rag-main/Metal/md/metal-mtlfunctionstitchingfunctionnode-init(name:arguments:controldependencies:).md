

- Metal
- MTLFunctionStitchingFunctionNode
-  init(name:arguments:controlDependencies:) 

Initializer

# init(name:arguments:controlDependencies:)

Creates a new function node.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
init(
    name: String,
    arguments: [any MTLFunctionStitchingNode],
    controlDependencies: [MTLFunctionStitchingFunctionNode]
)
```

## Parameters 

`name`  

The name of the function to call.

`arguments`  

An ordered list of the nodes that provide the function’s arguments.

`controlDependencies`  

The list of nodes that must execute before executing this node.

