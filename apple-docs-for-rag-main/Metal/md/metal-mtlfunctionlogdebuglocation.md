

- Metal
-  MTLFunctionLogDebugLocation 

Protocol

# MTLFunctionLogDebugLocation

The source code that logged a debug message.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
protocol MTLFunctionLogDebugLocation : NSObjectProtocol
```

## Topics

### Inspecting the Location Details

var functionName: String?

The name of the shader function.

**Required**

var url: URL?

The URL of the file that contains the shader function.

**Required**

var line: Int

The line that the log message appears on.

**Required**

var column: Int

The column where the log message appears.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

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

