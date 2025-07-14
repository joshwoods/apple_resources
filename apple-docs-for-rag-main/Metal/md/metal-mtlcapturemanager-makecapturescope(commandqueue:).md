

- Metal
- MTLCaptureManager
-  makeCaptureScope(commandQueue:) 

Instance Method

# makeCaptureScope(commandQueue:)

Creates a capture scope for commands submitted to a specific command queue.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func makeCaptureScope(commandQueue: any MTLCommandQueue) -> any MTLCaptureScope
```

## Parameters 

`commandQueue`  

The command queue whose commands you want to capture.

## See Also

### Creating a Capture Scope

func makeCaptureScope(device: any MTLDevice) -> any MTLCaptureScope

Creates a capture scope for commands submitted to a specific device object.

var defaultCaptureScope: (any MTLCaptureScope)?

The capture scope to use when a capture is initiated in Xcode.

