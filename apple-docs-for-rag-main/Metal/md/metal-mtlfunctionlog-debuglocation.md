

- Metal
- MTLFunctionLog
-  debugLocation 

Instance Property

# debugLocation

If known, the location of the logging command within a shader source file.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var debugLocation: (any MTLFunctionLogDebugLocation)? { get }
```

**Required**

## See Also

### Getting Execution Details

var encoderLabel: String?

The label for the encoder that logged the message.

**Required**

var function: (any MTLFunction)?

When known, the function object corresponding to the logged message.

**Required**

protocol MTLFunctionLogDebugLocation

The source code that logged a debug message.

