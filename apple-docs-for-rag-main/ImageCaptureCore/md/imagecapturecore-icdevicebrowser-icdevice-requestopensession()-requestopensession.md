

- ImageCaptureCore
- ICDeviceBrowser
- ICDevice
-  requestOpenSession() 

Instance Method

# requestOpenSession()

Requests to open a session on the device.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
func requestOpenSession()
```

## Discussion

Set the receiver’s delegate before calling this method; otherwise, the request is ignored.

Once the request to open the session has completed, device(_:didOpenSessionWithError:) is called on the delegate.

Execution of the delegate callback occurs on the main thread.

## See Also

### Managing a Device

var delegate: (any ICDeviceDelegate)?

The delegate to receive messages once a session is opened on the device.

protocol ICDeviceDelegate

Methods for responding to device events and changes.

var hasOpenSession: Bool

A Boolean value that indicates whether the device has an open session.

func requestOpenSession(options: [ICSessionOptions : Any]?, completion: ((any Error)?) -> Void)

Requests to open a session on the device, then executes the completion handler.

func requestSendMessage(UInt32, outData: Data, maxReturnedDataSize: UInt32, sendMessageDelegate: Any, didSendMessageSelector: Selector, contextInfo: UnsafeMutableRawPointer?)

Asynchronously sends an arbitrary message with optional data to a device.

func requestCloseSession()

Requests to close an open session on the device.

func requestCloseSession(options: [ICSessionOptions : Any]?, completion: ((any Error)?) -> Void)

Requests to close an open session on the device, then executes the completion handler.

func requestEject()

Requests to eject the media if permitted by the device, or to disconnect from a remote device.

func requestEject(completion: ((any Error)?) -> Void)

Requests to eject the media if permitted by the device, or to disconnect from a remote device, then executes the completion handler.

