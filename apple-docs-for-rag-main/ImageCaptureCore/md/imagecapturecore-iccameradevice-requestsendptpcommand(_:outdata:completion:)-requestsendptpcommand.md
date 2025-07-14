

- ImageCaptureCore
- ICCameraDevice
-  requestSendPTPCommand(\_:outData:completion:) 

Instance Method

# requestSendPTPCommand(\_:outData:completion:)

Sends a Picture Transfer Protocol (PTP) command to a camera asynchronously.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func requestSendPTPCommand(
    _ ptpCommand: Data,
    outData ptpData: Data?,
    completion: @escaping (Data, Data, (any Error)?) -> Void
)
```

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

The block receives the response, data, and an error message, if present.

## See Also

### Taking Pictures

var tetheredCaptureEnabled: Bool

A Boolean value indicating whether tethered capture is enabled on the camera.

var ptpEventHandler: (Data) -> Void

A closure for handling PTP event packets.

func requestEnableTethering()

Enables tethered capture if the camera has the capability to take pictures while connected.

Deprecated

func requestTakePicture()

Captures a new image using the camera.

func requestSendPTPCommand(Data, outData: Data?, sendCommandDelegate: Any, didSendCommand: Selector, contextInfo: UnsafeMutableRawPointer?)

Sends a Picture Transfer Protocol (PTP) command to a camera asynchronously.

func requestDisableTethering()

Disables tethered capture on the camera.

Deprecated

