

- ImageCaptureCore
- ICCameraDevice
-  requestEnableTethering() Deprecated

Instance Method

# requestEnableTethering()

Enables tethered capture if the camera has the capability to take pictures while connected.

macOS 10.4–14.0Deprecated

``` source
func requestEnableTethering()
```

## Discussion

To confirm whether a camera can take pictures while connected, check whether its capabilities include cameraDeviceCanTakePicture.

## See Also

### Taking Pictures

var tetheredCaptureEnabled: Bool

A Boolean value indicating whether tethered capture is enabled on the camera.

var ptpEventHandler: (Data) -> Void

A closure for handling PTP event packets.

func requestTakePicture()

Captures a new image using the camera.

func requestSendPTPCommand(Data, outData: Data?, sendCommandDelegate: Any, didSendCommand: Selector, contextInfo: UnsafeMutableRawPointer?)

Sends a Picture Transfer Protocol (PTP) command to a camera asynchronously.

func requestSendPTPCommand(Data, outData: Data?, completion: (Data, Data, (any Error)?) -> Void)

Sends a Picture Transfer Protocol (PTP) command to a camera asynchronously.

func requestDisableTethering()

Disables tethered capture on the camera.

Deprecated

