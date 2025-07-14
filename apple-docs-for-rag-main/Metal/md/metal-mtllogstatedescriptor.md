

- Metal
-  MTLLogStateDescriptor 

Class

# MTLLogStateDescriptor

An interface that represents a log state configuration.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
class MTLLogStateDescriptor
```

## Mentioned in 

Logging shader debug messages

## Overview

Configure the descriptor to create an MTLLogState by calling makeLogState(descriptor:).

If you’ve set the environment variables `MTL_LOG_BUFFER_SIZE` or `MTL_LOG_LEVEL`, then the system automatically enables logging. If any command buffer or command queue has an attached log state, then the system uses the log state’s settings instead of the environment variable values.

## Topics

### Instance Properties

var bufferSize: Int

The size of the internal buffer the log state uses, specified in bytes.

var level: MTLLogLevel

The minimum level of messages that the shader can log.

### Log Levels

enum MTLLogLevel

The supported log levels for shader logging.

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

### Shader Logging

protocol MTLLogState

A container for shader log messages.

