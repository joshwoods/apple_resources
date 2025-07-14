

- ImageCaptureCore
-  ICDeviceDelegate 

Protocol

# ICDeviceDelegate

Methods for responding to device events and changes.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
protocol ICDeviceDelegate : NSObjectProtocol
```

## Overview

Unless otherwise noted, all completion blocks execute on the calling thread.

## Topics

### Responding to Device Events

func device(ICDevice, didOpenSessionWithError: (any Error)?)

Tells the delegate when a session is opened on a device.

**Required**

func device(ICDevice, didCloseSessionWithError: (any Error)?)

Tells the delegate when a session is closed on a device.

**Required**

func didRemove(ICDevice)

Tells the delegate that a device has been removed.

**Required**

func deviceDidBecomeReady(ICDevice)

Tells the delegate when the device is ready to receive requests.

func device(ICDevice, didReceiveStatusInformation: [ICDeviceStatus : Any])

Tells the delegate when status information is received from a device.

func device(ICDevice, didEncounterError: (any Error)?)

Tells the delegate when a device encounters an error.

func device(ICDevice, didEjectWithError: (any Error)?)

Tells the delegate when the ejection is complete.

### Responding to Device Changes

func deviceDidChangeName(ICDevice)

Tells the delegate when the name of a device changes.

func deviceDidChangeSharingState(ICDevice)

Tells the delegate when the sharing state of a device changes.

Deprecated

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- ICCameraDeviceDelegate
- ICScannerDeviceDelegate

## See Also

### Managing a Device

var delegate: (any ICDeviceDelegate)?

The delegate to receive messages once a session is opened on the device.

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

func requestEject(completion: ((any Error)?) -> Void)

Requests to eject the media if permitted by the device, or to disconnect from a remote device, then executes the completion handler.

