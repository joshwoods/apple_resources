

- SceneKit
-  SCNBufferBindingBlock 

Type Alias

# SCNBufferBindingBlock

A block SceneKit calls at render time for working with buffers in a Metal shader, used by the handleBinding(ofBufferNamed:frequency:handler:) method.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias SCNBufferBindingBlock = (any SCNBufferStream, SCNNode, any SCNShadable, SCNRenderer) -> Void
```

## Discussion

The block takes the following parameters:

buffer  
An object that provides write access to the buffer. Use the writeBytes(_:count:) method on this object to write data for use by the shader.

node  
The node to be rendered using the shader program.

shadable  
The material or geometry to be rendered using the shader program.

renderer  
The view (or other SceneKit renderer) responsible for rendering.

## See Also

### Providing Input for Metal Shaders

func handleBinding(ofBufferNamed: String, frequency: SCNBufferFrequency, handler: SCNBufferBindingBlock)

Registers a block for SceneKit to call at render time for binding a Metal buffer to the shader program.

enum SCNBufferFrequency

Options for how often SceneKit should execute the binding handler you provide with the handleBinding(ofBufferNamed:frequency:handler:) method.

