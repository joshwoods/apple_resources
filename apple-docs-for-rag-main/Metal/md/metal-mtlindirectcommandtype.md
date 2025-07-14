

- Metal
-  MTLIndirectCommandType 

Structure

# MTLIndirectCommandType

The types of commands that you can encode into the indirect command buffer.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
struct MTLIndirectCommandType
```

## Topics

### Creating a Set of Command Types

init(rawValue: UInt)

Initializes the set of command types from a raw integer value.

### Specifying Command Types

static var draw: MTLIndirectCommandType

A draw call command.

static var drawIndexed: MTLIndirectCommandType

An indexed draw call command.

static var drawPatches: MTLIndirectCommandType

A draw call command for tessellated patches.

static var drawIndexedPatches: MTLIndirectCommandType

An indexed draw call command for tessellated patches.

static var concurrentDispatch: MTLIndirectCommandType

A compute command using a grid aligned to threadgroup boundaries.

static var concurrentDispatchThreads: MTLIndirectCommandType

A compute command using an arbitrarily sized grid.

### Type Properties

static var drawMeshThreadgroups: MTLIndirectCommandType

static var drawMeshThreads: MTLIndirectCommandType

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

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

struct MTLIndirectCommandBufferExecutionRange

A range of commands in an indirect command buffer.

func MTLIndirectCommandBufferExecutionRangeMake(UInt32, UInt32) -> MTLIndirectCommandBufferExecutionRange

Creates a command execution range.

