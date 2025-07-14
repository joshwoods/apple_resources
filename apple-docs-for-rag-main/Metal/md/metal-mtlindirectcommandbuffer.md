

- Metal
-  MTLIndirectCommandBuffer 

Protocol

# MTLIndirectCommandBuffer

A command buffer containing reusable commands, encoded either on the CPU or GPU.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
protocol MTLIndirectCommandBuffer : MTLResource
```

## Mentioned in 

Improving CPU Performance by Using Argument Buffers

## Overview

Use an indirect command buffer to encode commands once and reuse them, and to encode commands on multiple CPU or GPU threads.

Don’t implement this protocol yourself; instead, create a MTLIndirectCommandBufferDescriptor object, configure its properties, and tell the MTLDevice to create the indirect command buffer. See Creating an Indirect Command Buffer.

## Topics

### Determining the Maximum Number of Commands

var size: Int

The number of commands contained in the indirect command buffer.

**Required**

### Retrieving Commands

func indirectRenderCommandAt(Int) -> any MTLIndirectRenderCommand

Gets the render command at the given index.

**Required**

func indirectComputeCommandAt(Int) -> any MTLIndirectComputeCommand

Gets the compute command at the given index.

**Required**

func indirectComputeCommand(at: Int) -> any MTLIndirectComputeCommand

Gets the compute command at the given index.

### Resetting Commands

func reset(Range&lt;Int>)

Resets a range of commands to their default state.

### Instance Properties

var gpuResourceID: MTLResourceID

**Required**

## Relationships

### Inherits From

- MTLAllocation
- MTLResource
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

class MTLIndirectCommandBufferDescriptor

A configuration you create to customize an indirect command buffer.

struct MTLIndirectCommandType

The types of commands that you can encode into the indirect command buffer.

struct MTLIndirectCommandBufferExecutionRange

A range of commands in an indirect command buffer.

func MTLIndirectCommandBufferExecutionRangeMake(UInt32, UInt32) -> MTLIndirectCommandBufferExecutionRange

Creates a command execution range.

