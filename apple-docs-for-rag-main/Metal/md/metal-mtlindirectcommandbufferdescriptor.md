

- Metal
-  MTLIndirectCommandBufferDescriptor 

Class

# MTLIndirectCommandBufferDescriptor

A configuration you create to customize an indirect command buffer.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
class MTLIndirectCommandBufferDescriptor
```

## Mentioned in 

Creating an Indirect Command Buffer

## Topics

### Declaring Command Types to Encode

var commandTypes: MTLIndirectCommandType

The set of command types that you can encode into the indirect command buffer.

### Declaring Command Inheritance

var inheritBuffers: Bool

A Boolean value that determines where commands in the indirect command buffer get their buffer arguments from when you execute them.

var inheritPipelineState: Bool

A Boolean value that determines where commands in the indirect command buffer get their pipeline state from when you execute them.

### Declaring the Maximum Number of Argument Buffers Per Command

var maxVertexBufferBindCount: Int

The maximum number of buffers that you can set per command for the vertex stage.

var maxFragmentBufferBindCount: Int

The maximum number of buffers that you can set per command for the fragment stage.

var maxKernelBufferBindCount: Int

The maximum number of buffers that you can set per command for the compute kernel.

### Instance Properties

var maxKernelThreadgroupMemoryBindCount: Int

var maxMeshBufferBindCount: Int

var maxObjectBufferBindCount: Int

var maxObjectThreadgroupMemoryBindCount: Int

var supportDynamicAttributeStride: Bool

var supportRayTracing: Bool

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Indirect Command Buffers

Creating an Indirect Command Buffer

Configure a descriptor to specify the properties of an indirect command buffer.

Specifying Drawing and Dispatch Arguments Indirectly

Use indirect commands if you don’t know your draw or dispatch call arguments when you encode the command.

Encoding Indirect Command Buffers on the CPU

Reduce CPU overhead and simplify your command execution by reusing commands.

Encoding Indirect Command Buffers on the GPU

Maximize CPU to GPU parallelization by generating render commands on the GPU.

protocol MTLIndirectCommandBuffer

A command buffer containing reusable commands, encoded either on the CPU or GPU.

struct MTLIndirectCommandType

The types of commands that you can encode into the indirect command buffer.

struct MTLIndirectCommandBufferExecutionRange

A range of commands in an indirect command buffer.

func MTLIndirectCommandBufferExecutionRangeMake(UInt32, UInt32) -> MTLIndirectCommandBufferExecutionRange

Creates a command execution range.

