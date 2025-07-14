

- Metal
- MTLIndirectCommandBufferDescriptor
-  maxVertexBufferBindCount 

Instance Property

# maxVertexBufferBindCount

The maximum number of buffers that you can set per command for the vertex stage.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
var maxVertexBufferBindCount: Int { get set }
```

## Discussion

Metal ignores this property if inheritBuffers is true or if you configured commandTypes for compute commands. Metal must reserve enough memory in each command to store this many arguments. Use the smallest value that works for all commands you plan to encode into the indirect command buffer.

## See Also

### Declaring the Maximum Number of Argument Buffers Per Command

var maxFragmentBufferBindCount: Int

The maximum number of buffers that you can set per command for the fragment stage.

var maxKernelBufferBindCount: Int

The maximum number of buffers that you can set per command for the compute kernel.

