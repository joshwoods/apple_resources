

- Metal
-  MTLIndirectCommandBufferExecutionRange 

Structure

# MTLIndirectCommandBufferExecutionRange

A range of commands in an indirect command buffer.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.14+tvOS 13.0+visionOS 1.0+

``` source
struct MTLIndirectCommandBufferExecutionRange
```

## Topics

### Creating a Command Execution Range

init()

Initializes an empty command execution range.

init(location: UInt32, length: UInt32)

Initializes an command execution range.

func MTLIndirectCommandBufferExecutionRangeMake(UInt32, UInt32) -> MTLIndirectCommandBufferExecutionRange

Creates a command execution range.

### Examining the Range

var location: UInt32

The first index in the command execution range.

var length: UInt32

The number of items in the command execution range.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

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

class MTLIndirectCommandBufferDescriptor

A configuration you create to customize an indirect command buffer.

struct MTLIndirectCommandType

The types of commands that you can encode into the indirect command buffer.

func MTLIndirectCommandBufferExecutionRangeMake(UInt32, UInt32) -> MTLIndirectCommandBufferExecutionRange

Creates a command execution range.

