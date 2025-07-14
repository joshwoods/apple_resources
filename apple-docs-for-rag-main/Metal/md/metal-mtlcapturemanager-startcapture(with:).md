

- Metal
- MTLCaptureManager
-  startCapture(with:) 

Instance Method

# startCapture(with:)

Starts capturing any of your app’s Metal commands, with the capture session defined by a descriptor object.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
func startCapture(with descriptor: MTLCaptureDescriptor) throws
```

## Parameters 

`descriptor`  

A description of the capture session to create.

## See Also

### Starting Capture

func startCapture(device: any MTLDevice)

Starts capturing any of your app’s Metal commands that are executed by the device object.

Deprecated

func startCapture(commandQueue: any MTLCommandQueue)

Starts capturing any of your app’s Metal commands that are executed by the command queue.

Deprecated

func startCapture(scope: any MTLCaptureScope)

Starts capturing any of your app’s Metal commands that are in the specified capture scope.

Deprecated

