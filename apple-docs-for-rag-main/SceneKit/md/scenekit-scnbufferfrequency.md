

- SceneKit
-  SCNBufferFrequency 

Enumeration

# SCNBufferFrequency

Options for how often SceneKit should execute the binding handler you provide with the handleBinding(ofBufferNamed:frequency:handler:) method.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum SCNBufferFrequency
```

## Topics

### Constants

case perFrame

Execute the binding handler once for each frame to be rendered using the shader.

case perNode

Execute the binding handler once for each frame, for each node to be rendered using the shader.

case perShadable

Execute the binding handler once for each frame, for each node, for each material or geometry to be rendered using the shader.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Providing Input for Metal Shaders

func handleBinding(ofBufferNamed: String, frequency: SCNBufferFrequency, handler: SCNBufferBindingBlock)

Registers a block for SceneKit to call at render time for binding a Metal buffer to the shader program.

typealias SCNBufferBindingBlock

A block SceneKit calls at render time for working with buffers in a Metal shader, used by the handleBinding(ofBufferNamed:frequency:handler:) method.

