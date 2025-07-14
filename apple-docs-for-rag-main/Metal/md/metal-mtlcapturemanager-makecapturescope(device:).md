

- Metal
- MTLCaptureManager
-  makeCaptureScope(device:) 

Instance Method

# makeCaptureScope(device:)

Creates a capture scope for commands submitted to a specific device object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func makeCaptureScope(device: any MTLDevice) -> any MTLCaptureScope
```

## Parameters 

`device`  

The device object whose commands you want to capture.

## Discussion

The capture scope captures commands in command buffers created on any command queues created by the device object.

## See Also

### Creating a Capture Scope

func makeCaptureScope(commandQueue: any MTLCommandQueue) -> any MTLCaptureScope

Creates a capture scope for commands submitted to a specific command queue.

var defaultCaptureScope: (any MTLCaptureScope)?

The capture scope to use when a capture is initiated in Xcode.

