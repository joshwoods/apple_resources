

- ImageCaptureCore
- ICDeviceBrowser
- ICDevice
- ICDeviceDelegate
-  device(\_:didCloseSessionWithError:) 

Instance Method

# device(\_:didCloseSessionWithError:)

Tells the delegate when a session is closed on a device.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
func device(
    _ device: ICDevice,
    didCloseSessionWithError error: (any Error)?
)
```

**Required**

## Discussion

This message completes the process initiated by the message "requestCloseSession" sent to the device object. This message is also sent if the device module in control of the device ceases to control the device.

Execution of the delegate callback occurs on the main thread.

## See Also

### Responding to Device Events

func device(ICDevice, didOpenSessionWithError: (any Error)?)

Tells the delegate when a session is opened on a device.

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

