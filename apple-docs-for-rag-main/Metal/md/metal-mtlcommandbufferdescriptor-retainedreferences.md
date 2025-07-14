

- Metal
- MTLCommandBufferDescriptor
-  retainedReferences 

Instance Property

# retainedReferences

A Boolean value that indicates whether the command buffer the descriptor creates maintains strong references to the resources it uses.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var retainedReferences: Bool { get set }
```

## Discussion

Set this property to true (its default) to create a command buffer that maintains strong references to resource instances that its commands need. Otherwise, set it to false to create a command buffer that doesn’t maintain strong references to its resources.

Apps typically create command buffers that don’t maintain references to resources for extremely performance-critical situations. Even though the runtime cost for retaining or releasing a single resource is trivial, the aggregate time savings may be worth it.

It’s your app’s responsibility to maintain strong references to all the resources the command buffer uses until it finishes running on the GPU.

Important

Releasing a resource before a command buffer’s commands complete may trigger a runtime error or erratic behavior.

You can determine whether an existing command buffer retains references by checking its retainedReferences property.

## See Also

### Configuring the Command Buffer

var logState: (any MTLLogState)?

The shader logging configuration that the command buffer uses.

var errorOptions: MTLCommandBufferErrorOption

The reporting configuration that indicates which information the GPU driver stores in a command buffer’s error property.

struct MTLCommandBufferErrorOption

Options for reporting errors from a command buffer.

