

- Metal
- Indirect Command Encoding
-  Creating an Indirect Command Buffer 

Article

# Creating an Indirect Command Buffer

Configure a descriptor to specify the properties of an indirect command buffer.

## Overview

An indirect command buffer stores encoded GPU commands persistently. Using an indirect command buffer, you can encode a command once and reuse it multiple times. You can also encode commands into an indirect command buffer simultaneously with multiple threads on the CPU or with a compute kernel on the GPU.

To create an indirect command buffer, first create a MTLIndirectCommandBufferDescriptor object and configure the descriptor’s properties. Then call makeIndirectCommandBuffer(descriptor:maxCommandCount:options:) on a MTLDevice object to create the indirect command buffer.

## See Also

### Indirect Command Buffers

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

struct MTLIndirectCommandBufferExecutionRange

A range of commands in an indirect command buffer.

func MTLIndirectCommandBufferExecutionRangeMake(UInt32, UInt32) -> MTLIndirectCommandBufferExecutionRange

Creates a command execution range.

