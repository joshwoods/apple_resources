

- ImageCaptureCore
- ICCameraDevice
-  requestTakePicture() 

Instance Method

# requestTakePicture()

Captures a new image using the camera.

macOS 10.4+

``` source
func requestTakePicture()
```

## Discussion

Before taking a picture, you must first enable tethering by calling requestEnableTethering().

## See Also

### Taking Pictures

var tetheredCaptureEnabled: Bool

A Boolean value indicating whether tethered capture is enabled on the camera.

var ptpEventHandler: (Data) -> Void

A closure for handling PTP event packets.

func requestEnableTethering()

Enables tethered capture if the camera has the capability to take pictures while connected.

Deprecated

func requestSendPTPCommand(Data, outData: Data?, sendCommandDelegate: Any, didSendCommand: Selector, contextInfo: UnsafeMutableRawPointer?)

Sends a Picture Transfer Protocol (PTP) command to a camera asynchronously.

func requestSendPTPCommand(Data, outData: Data?, completion: (Data, Data, (any Error)?) -> Void)

Sends a Picture Transfer Protocol (PTP) command to a camera asynchronously.

func requestDisableTethering()

Disables tethered capture on the camera.

Deprecated

