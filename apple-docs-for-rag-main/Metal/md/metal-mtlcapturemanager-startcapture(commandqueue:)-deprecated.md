

- Metal
- MTLCaptureManager
-  startCapture(commandQueue:) Deprecated

Instance Method

# startCapture(commandQueue:)

Starts capturing any of your app’s Metal commands that are executed by the command queue.

iOS 11.0–13.0DeprecatediPadOS 11.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.13–10.15DeprecatedtvOS 11.0–13.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func startCapture(commandQueue: any MTLCommandQueue)
```

Deprecated

Use startCapture(with:) instead.

## Parameters 

`commandQueue`  

The command queue whose commands you want to capture.

## See Also

### Starting Capture

func startCapture(with: MTLCaptureDescriptor) throws

Starts capturing any of your app’s Metal commands, with the capture session defined by a descriptor object.

func startCapture(device: any MTLDevice)

Starts capturing any of your app’s Metal commands that are executed by the device object.

Deprecated

func startCapture(scope: any MTLCaptureScope)

Starts capturing any of your app’s Metal commands that are in the specified capture scope.

Deprecated

