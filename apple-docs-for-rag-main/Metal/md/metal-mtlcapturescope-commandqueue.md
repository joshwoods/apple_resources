

- Metal
- MTLCaptureScope
-  commandQueue 

Instance Property

# commandQueue

The command queue that this capture scope uses to limit which commands are recorded.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var commandQueue: (any MTLCommandQueue)? { get }
```

**Required**

## Discussion

This value is only available if you created the capture scope by calling the makeCaptureScope(commandQueue:) method. Otherwise, the value is `nil`.

## See Also

### Identifying the Capture Scope

var label: String?

A string that identifies the capture scope.

**Required**

var device: any MTLDevice

The device object from which you created the capture scope.

**Required**

