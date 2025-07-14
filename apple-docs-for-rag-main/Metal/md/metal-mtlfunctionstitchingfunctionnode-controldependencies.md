

- Metal
- MTLFunctionStitchingFunctionNode
-  controlDependencies 

Instance Property

# controlDependencies

The list of nodes that must execute before executing the node.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var controlDependencies: [MTLFunctionStitchingFunctionNode] { get set }
```

## Discussion

When a stitched function calls functions that have side effects on their input data, you often need the GPU to execute functions in a specific order. In such cases, use the controlDependencies property to specify which nodes must execute before executing this node.

## See Also

### Configuring a Function Node

var name: String

The name of the function to call.

var arguments: [any MTLFunctionStitchingNode]

An ordered list of the nodes that provide the function’s arguments.

