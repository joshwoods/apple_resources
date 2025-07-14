

- ImageCaptureCore
- ICCameraDevice
-  tetheredCaptureEnabled 

Instance Property

# tetheredCaptureEnabled

A Boolean value indicating whether tethered capture is enabled on the camera.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
var tetheredCaptureEnabled: Bool { get }
```

## Discussion

Use requestEnableTethering() and requestDisableTethering() to enable or disable tethered capture.

## See Also

### Taking Pictures

var ptpEventHandler: (Data) -> Void

A closure for handling PTP event packets.

func requestEnableTethering()

Enables tethered capture if the camera has the capability to take pictures while connected.

Deprecated

func requestTakePicture()

Captures a new image using the camera.

func requestSendPTPCommand(Data, outData: Data?, sendCommandDelegate: Any, didSendCommand: Selector, contextInfo: UnsafeMutableRawPointer?)

Sends a Picture Transfer Protocol (PTP) command to a camera asynchronously.

func requestSendPTPCommand(Data, outData: Data?, completion: (Data, Data, (any Error)?) -> Void)

Sends a Picture Transfer Protocol (PTP) command to a camera asynchronously.

func requestDisableTethering()

Disables tethered capture on the camera.

Deprecated

