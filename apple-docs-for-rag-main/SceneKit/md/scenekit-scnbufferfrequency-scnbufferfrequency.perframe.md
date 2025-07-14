

- SceneKit
- SCNBufferFrequency
-  SCNBufferFrequency.perFrame 

Case

# SCNBufferFrequency.perFrame

Execute the binding handler once for each frame to be rendered using the shader.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case perFrame
```

## Discussion

Use this option when the contents of the buffer should be uniform across all uses of the shader when rendering a single frame, no matter how many different nodes, geometries, and materials use the shader program.

## See Also

### Constants

case perNode

Execute the binding handler once for each frame, for each node to be rendered using the shader.

case perShadable

Execute the binding handler once for each frame, for each node, for each material or geometry to be rendered using the shader.

