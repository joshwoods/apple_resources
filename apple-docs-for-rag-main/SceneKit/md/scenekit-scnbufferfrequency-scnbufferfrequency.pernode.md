

- SceneKit
- SCNBufferFrequency
-  SCNBufferFrequency.perNode 

Case

# SCNBufferFrequency.perNode

Execute the binding handler once for each frame, for each node to be rendered using the shader.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case perNode
```

## Discussion

Use this option when the contents of the buffer should be uniform across multiple geometries or materials, but specific to each node rendered using the shader. For example, a node-specific buffer might contain information based on the node’s position and transform.

## See Also

### Constants

case perFrame

Execute the binding handler once for each frame to be rendered using the shader.

case perShadable

Execute the binding handler once for each frame, for each node, for each material or geometry to be rendered using the shader.

