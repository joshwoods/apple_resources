

- Metal
-  MTLCommandBufferEncoderInfo 

Protocol

# MTLCommandBufferEncoderInfo

A container that provides additional information about a runtime failure a GPU encounters as it runs the commands in a command buffer.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
protocol MTLCommandBufferEncoderInfo : NSObjectProtocol
```

## Overview

To create a command buffer that generates additional information (when a GPU encounters an error running it), configure an MTLCommandBufferDescriptor instance’s errorOptions property. For information about how to retrieve the information from an MTLCommandBuffer instance, see its error property.

## Topics

### Inspecting Execution Information

var label: String

The name of the encoder that generates the error information.

**Required**

var debugSignposts: [String]

An array of debug signposts that Metal records as the GPU executes the commands of the encoder’s pass.

**Required**

var errorState: MTLCommandEncoderErrorState

The execution status of the command encoder.

**Required**

enum MTLCommandEncoderErrorState

Possible error conditions for the command encoder’s commands.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Getting Error Details

var error: (any Error)?

A description of an error when the GPU encounters an issue as it runs the command buffer.

**Required**

var errorOptions: MTLCommandBufferErrorOption

Settings that determine which information the command buffer records about execution errors, and how it does it.

**Required**

let MTLCommandBufferEncoderInfoErrorKey: String

A key to a command buffer error’s user information dictionary that retrieves additional information about a GPU’s runtime error.

