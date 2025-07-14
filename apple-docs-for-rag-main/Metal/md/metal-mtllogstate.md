

- Metal
-  MTLLogState 

Protocol

# MTLLogState

A container for shader log messages.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
protocol MTLLogState : NSObjectProtocol
```

## Mentioned in 

Logging shader debug messages

## Overview

Create an MTLCommandQueue or MTLCommandBuffer with a log state to hold messages logged from shaders. Attach a log state to a command buffer by assigning it to the command buffer descriptor’s logState. Similarly, to attach a log state to a command queue, use the command queue descriptor’s logState.

When you attach a log state to a command queue, the command queue shares the log state with all the command buffers it creates. If you attach different log states to a command buffer and command queue, then the system uses the state attached to the command buffer.

Because logging incurs an overhead, regardless of whether the system prints messages, you must explicitly enable logging with enableLogging.

## Topics

### Instance Methods

func addLogHandler((String?, String?, MTLLogLevel, String) -> Void)

Adds a log handler to customize the presentation of shader logging.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Shader Logging

class MTLLogStateDescriptor

An interface that represents a log state configuration.

