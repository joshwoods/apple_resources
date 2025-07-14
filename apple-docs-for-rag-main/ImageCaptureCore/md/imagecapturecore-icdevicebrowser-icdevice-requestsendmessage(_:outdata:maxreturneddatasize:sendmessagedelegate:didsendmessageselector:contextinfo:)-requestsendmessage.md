

- ImageCaptureCore
- ICDeviceBrowser
- ICDevice
-  requestSendMessage(\_:outData:maxReturnedDataSize:sendMessageDelegate:didSendMessageSelector:contextInfo:) 

Instance Method

# requestSendMessage(\_:outData:maxReturnedDataSize:sendMessageDelegate:didSendMessageSelector:contextInfo:)

Asynchronously sends an arbitrary message with optional data to a device.

macOS 10.4+

``` source
func requestSendMessage(
    _ messageCode: UInt32,
    outData data: Data,
    maxReturnedDataSize: UInt32,
    sendMessageDelegate: Any,
    didSendMessageSelector selector: Selector,
    contextInfo: UnsafeMutableRawPointer?
)
```

## Discussion

Use this method to send a private message from a client application to a device module.

The `sendMessageDelegate` must implement a function with the signature `(void)didSendMessage:(UInt32)messageCode inData:(NSData*)data error:(NSError*)error contextInfo:(void*)contextInfo`, to be called when the request is completed.

Do not use this method to send PTP pass-through commands to a PTP camera. Use requestSendPTPCommand(_:outData:sendCommandDelegate:didSendCommand:contextInfo:) instead.

Execution of the delegate callback occurs on the main thread.

## See Also

### Managing a Device

var delegate: (any ICDeviceDelegate)?

The delegate to receive messages once a session is opened on the device.

protocol ICDeviceDelegate

Methods for responding to device events and changes.

var hasOpenSession: Bool

A Boolean value that indicates whether the device has an open session.

func requestOpenSession()

Requests to open a session on the device.

func requestOpenSession(options: [ICSessionOptions : Any]?, completion: ((any Error)?) -> Void)

Requests to open a session on the device, then executes the completion handler.

func requestCloseSession()

Requests to close an open session on the device.

func requestCloseSession(options: [ICSessionOptions : Any]?, completion: ((any Error)?) -> Void)

Requests to close an open session on the device, then executes the completion handler.

func requestEject()

Requests to eject the media if permitted by the device, or to disconnect from a remote device.

func requestEject(completion: ((any Error)?) -> Void)

Requests to eject the media if permitted by the device, or to disconnect from a remote device, then executes the completion handler.

