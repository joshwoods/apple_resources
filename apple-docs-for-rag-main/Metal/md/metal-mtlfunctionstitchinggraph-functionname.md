

- Metal
- MTLFunctionStitchingGraph
-  functionName 

Instance Property

# functionName

The name of the new stitched function.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var functionName: String { get set }
```

## See Also

### Configuring a Function Graph

var nodes: [MTLFunctionStitchingFunctionNode]

The nodes in the function’s call graph.

var outputNode: MTLFunctionStitchingFunctionNode?

The node with the output that’s the output of the new stitched function.

var attributes: [any MTLFunctionStitchingAttribute]

A list of attributes to configure how the Metal device object generates the new stitched function.

