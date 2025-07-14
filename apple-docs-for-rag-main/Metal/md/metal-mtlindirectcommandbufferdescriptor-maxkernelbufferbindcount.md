

- Metal
- MTLIndirectCommandBufferDescriptor
-  maxKernelBufferBindCount 

Instance Property

# maxKernelBufferBindCount

The maximum number of buffers that you can set per command for the compute kernel.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 11.0+tvOS 13.0+visionOS 1.0+

``` source
var maxKernelBufferBindCount: Int { get set }
```

## Discussion

Metal ignores this property if inheritBuffers is true or if you configured commandTypes for rendering commands. Metal must reserve enough memory in each command to store this many arguments. Use the smallest value that works for all commands you plan to encode into the indirect command buffer.

## See Also

### Declaring the Maximum Number of Argument Buffers Per Command

var maxVertexBufferBindCount: Int

The maximum number of buffers that you can set per command for the vertex stage.

var maxFragmentBufferBindCount: Int

The maximum number of buffers that you can set per command for the fragment stage.

