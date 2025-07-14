

- ImageCaptureCore
- ICDeviceBrowser
- ICDevice
-  requestEject(completion:) 

Instance Method

# requestEject(completion:)

Requests to eject the media if permitted by the device, or to disconnect from a remote device, then executes the completion handler.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func requestEject(completion: @escaping ((any Error)?) -> Void)
```

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

func requestEject() async throws

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Execution of the completion block occurs on the calling thread.

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

func requestSendMessage(UInt32, outData: Data, maxReturnedDataSize: UInt32, sendMessageDelegate: Any, didSendMessageSelector: Selector, contextInfo: UnsafeMutableRawPointer?)

Asynchronously sends an arbitrary message with optional data to a device.

func requestCloseSession()

Requests to close an open session on the device.

func requestCloseSession(options: [ICSessionOptions : Any]?, completion: ((any Error)?) -> Void)

Requests to close an open session on the device, then executes the completion handler.

func requestEject()

Requests to eject the media if permitted by the device, or to disconnect from a remote device.

