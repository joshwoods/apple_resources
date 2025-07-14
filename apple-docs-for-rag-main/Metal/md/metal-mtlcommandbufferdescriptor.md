

- Metal
-  MTLCommandBufferDescriptor 

Class

# MTLCommandBufferDescriptor

A configuration that customizes the behavior for a new command buffer.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class MTLCommandBufferDescriptor
```

## Overview

Create a command buffer with a custom configuration by creating an MTLCommandBufferDescriptor instance and passing it to an MTLCommandQueue instance’s makeCommandBuffer(descriptor:) method. You can configure whether the command buffer retains references to resources that its commands refer to with the retainedReferences property. The command buffer can save extra error information, which is useful during development, by setting its errorOptions property to encoderExecutionStatus.

## Topics

### Configuring the Command Buffer

var logState: (any MTLLogState)?

The shader logging configuration that the command buffer uses.

var retainedReferences: Bool

A Boolean value that indicates whether the command buffer the descriptor creates maintains strong references to the resources it uses.

var errorOptions: MTLCommandBufferErrorOption

The reporting configuration that indicates which information the GPU driver stores in a command buffer’s error property.

struct MTLCommandBufferErrorOption

Options for reporting errors from a command buffer.

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

### Submitting Work to a GPU

Setting Up a Command Structure

Discover how Metal executes commands on a GPU.

protocol MTLCommandQueue

An instance you use to create, submit, and schedule command buffers to a specific GPU device to run the commands within those buffers.

class MTLCommandQueueDescriptor

A configuration that customizes the behavior for a new command queue.

protocol MTLCommandBuffer

A container that stores a sequence of GPU commands that you encode into it.

struct MTLCommandBufferError

The command buffer error codes that indicate why the GPU doesn’t finish executing a command buffer.

protocol MTLCommandEncoder

An encoder that writes GPU commands into a command buffer.

