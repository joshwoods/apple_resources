

- SceneKit
- SCNProgram
-  handleBinding(ofBufferNamed:frequency:handler:) 

Instance Method

# handleBinding(ofBufferNamed:frequency:handler:)

Registers a block for SceneKit to call at render time for binding a Metal buffer to the shader program.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func handleBinding(
    ofBufferNamed name: String,
    frequency: SCNBufferFrequency,
    handler block: @escaping SCNBufferBindingBlock
)
```

## Parameters 

`name`  

The name identifying the buffer in Metal shader source code.

`frequency`  

An option specifying whether SceneKit calls the block only once per rendered frame or more frequently (for example, once for each object to be rendered).

`block`  

A block to be run when SceneKit prepares for rendering with the Metal shader.

## Discussion

Use this method to associate a block with a Metal shader program to handle setup of a buffer used in that shader. SceneKit calls your block before rendering any objects whose program property is set to this SCNProgram object. In the block, use the writeBytes(_:count:) method to provide data for the buffer.

## See Also

### Providing Input for Metal Shaders

enum SCNBufferFrequency

Options for how often SceneKit should execute the binding handler you provide with the handleBinding(ofBufferNamed:frequency:handler:) method.

typealias SCNBufferBindingBlock

A block SceneKit calls at render time for working with buffers in a Metal shader, used by the handleBinding(ofBufferNamed:frequency:handler:) method.

