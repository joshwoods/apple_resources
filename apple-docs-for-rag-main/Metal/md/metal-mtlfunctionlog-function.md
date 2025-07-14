

- Metal
- MTLFunctionLog
-  function 

Instance Property

# function

When known, the function object corresponding to the logged message.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var function: (any MTLFunction)? { get }
```

**Required**

## See Also

### Getting Execution Details

var debugLocation: (any MTLFunctionLogDebugLocation)?

If known, the location of the logging command within a shader source file.

**Required**

var encoderLabel: String?

The label for the encoder that logged the message.

**Required**

protocol MTLFunctionLogDebugLocation

The source code that logged a debug message.

