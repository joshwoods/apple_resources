

- ImageCaptureCore
- ICCameraDevice
-  requestSendPTPCommand(\_:outData:sendCommandDelegate:didSendCommand:contextInfo:) 

Instance Method

# requestSendPTPCommand(\_:outData:sendCommandDelegate:didSendCommand:contextInfo:)

Sends a Picture Transfer Protocol (PTP) command to a camera asynchronously.

iOS 15.2+iPadOS 15.2+Mac Catalyst 15.2+macOS 10.4+visionOS 1.0+

``` source
func requestSendPTPCommand(
    _ command: Data,
    outData data: Data?,
    sendCommandDelegate: Any,
    didSendCommand selector: Selector,
    contextInfo: UnsafeMutableRawPointer?
)
```

## Discussion

Call this method only if the capabilities property contains cameraDeviceCanAcceptPTPCommands. All PTP cameras have this capability.

The `sendCommandDelegate` must implement a function with the signature `- (void)didSendPTPCommand:(NSData*)command inData:(NSData*)data response:(NSData*)response error:(NSError*)error contextInfo:(void*)contextInfo`, to be called when the request is completed.

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

func requestSendPTPCommand(Data, outData: Data?, completion: (Data, Data, (any Error)?) -> Void)

Sends a Picture Transfer Protocol (PTP) command to a camera asynchronously.

func requestDisableTethering()

Disables tethered capture on the camera.

Deprecated

