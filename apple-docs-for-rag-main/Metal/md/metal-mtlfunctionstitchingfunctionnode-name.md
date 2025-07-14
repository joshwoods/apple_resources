

- Metal
- MTLFunctionStitchingFunctionNode
-  name 

Instance Property

# name

The name of the function to call.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var name: String { get set }
```

## Discussion

The name must match one of the functions in the stitched library descriptor’s functions property.

## See Also

### Configuring a Function Node

var arguments: [any MTLFunctionStitchingNode]

An ordered list of the nodes that provide the function’s arguments.

var controlDependencies: [MTLFunctionStitchingFunctionNode]

The list of nodes that must execute before executing the node.

