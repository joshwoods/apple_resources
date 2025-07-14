

- ImageCaptureCore
- ICCameraDevice
-  ptpEventHandler 

Instance Property

# ptpEventHandler

A closure for handling PTP event packets.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 12.0+visionOS 1.0+

``` source
var ptpEventHandler: (Data) -> Void { get set }
```

## Discussion

Set this property as an alternative to setting up an object to handle PTP event packets. If the handler is set, it is called in place of the delegate. If the handler is `nil`, the delegate is called, if present. If both are set, only the handler is called.

## See Also

### Taking Pictures

var tetheredCaptureEnabled: Bool

A Boolean value indicating whether tethered capture is enabled on the camera.

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

