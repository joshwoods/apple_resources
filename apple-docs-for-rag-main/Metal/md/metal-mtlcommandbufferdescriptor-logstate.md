

- Metal
- MTLCommandBufferDescriptor
-  logState 

Instance Property

# logState

The shader logging configuration that the command buffer uses.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var logState: (any MTLLogState)? { get set }
```

## See Also

### Configuring the Command Buffer

var retainedReferences: Bool

A Boolean value that indicates whether the command buffer the descriptor creates maintains strong references to the resources it uses.

var errorOptions: MTLCommandBufferErrorOption

The reporting configuration that indicates which information the GPU driver stores in a command buffer’s error property.

struct MTLCommandBufferErrorOption

Options for reporting errors from a command buffer.

