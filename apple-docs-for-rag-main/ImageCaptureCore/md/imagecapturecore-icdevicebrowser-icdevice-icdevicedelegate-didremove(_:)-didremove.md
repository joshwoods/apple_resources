

- ImageCaptureCore
- ICDeviceBrowser
- ICDevice
- ICDeviceDelegate
-  didRemove(\_:) 

Instance Method

# didRemove(\_:)

Tells the delegate that a device has been removed.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
func didRemove(_ device: ICDevice)
```

**Required**

## See Also

### Responding to Device Events

func device(ICDevice, didOpenSessionWithError: (any Error)?)

Tells the delegate when a session is opened on a device.

**Required**

func device(ICDevice, didCloseSessionWithError: (any Error)?)

Tells the delegate when a session is closed on a device.

**Required**

func deviceDidBecomeReady(ICDevice)

Tells the delegate when the device is ready to receive requests.

func device(ICDevice, didReceiveStatusInformation: [ICDeviceStatus : Any])

Tells the delegate when status information is received from a device.

func device(ICDevice, didEncounterError: (any Error)?)

Tells the delegate when a device encounters an error.

func device(ICDevice, didEjectWithError: (any Error)?)

Tells the delegate when the ejection is complete.

