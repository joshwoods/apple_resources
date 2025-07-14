

- Metal
-  MTLFunctionLog 

Protocol

# MTLFunctionLog

A log entry a Metal device generates when the it runs a command buffer.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
protocol MTLFunctionLog : NSObjectProtocol
```

## Topics

### Getting the Log Messsage

var type: MTLFunctionLogType

The type of message that was logged.

**Required**

enum MTLFunctionLogType

Options for different kinds of function logs.

### Getting Execution Details

var debugLocation: (any MTLFunctionLogDebugLocation)?

If known, the location of the logging command within a shader source file.

**Required**

var encoderLabel: String?

The label for the encoder that logged the message.

**Required**

var function: (any MTLFunction)?

When known, the function object corresponding to the logged message.

**Required**

protocol MTLFunctionLogDebugLocation

The source code that logged a debug message.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Shader Logs

struct MTLLogContainer

A collection of logged messages, created when a Metal device runs a command buffer.

