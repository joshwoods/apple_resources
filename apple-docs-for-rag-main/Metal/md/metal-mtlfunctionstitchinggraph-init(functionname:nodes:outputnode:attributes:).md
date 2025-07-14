

- Metal
- MTLFunctionStitchingGraph
-  init(functionName:nodes:outputNode:attributes:) 

Initializer

# init(functionName:nodes:outputNode:attributes:)

Creates a description of a new function call graph.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
init(
    functionName: String,
    nodes: [MTLFunctionStitchingFunctionNode],
    outputNode: MTLFunctionStitchingFunctionNode?,
    attributes: [any MTLFunctionStitchingAttribute]
)
```

## Parameters 

`functionName`  

The name of the new function.

`nodes`  

The nodes in the function’s call graph.

`outputNode`  

The node whose output is the output of the new stitched function.

`attributes`  

A list of attributes used to generate the new stitched function.

