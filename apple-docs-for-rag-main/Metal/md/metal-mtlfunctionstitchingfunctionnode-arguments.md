

- Metal
- MTLFunctionStitchingFunctionNode
-  arguments 

Instance Property

# arguments

An ordered list of the nodes that provide the function’s arguments.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var arguments: [any MTLFunctionStitchingNode] { get set }
```

## Discussion

The output data types of each of the nodes must match the input data type of the matching argument.

## See Also

### Configuring a Function Node

var name: String

The name of the function to call.

var controlDependencies: [MTLFunctionStitchingFunctionNode]

The list of nodes that must execute before executing the node.

