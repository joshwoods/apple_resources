

- ImageCaptureCore
-  ICDeviceBrowserDelegate 

Protocol

# ICDeviceBrowserDelegate

Methods for managing the addition and removal of devices and responding to device changes.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
protocol ICDeviceBrowserDelegate : NSObjectProtocol
```

## Topics

### Adding and Removing Devices

func deviceBrowser(ICDeviceBrowser, didAdd: ICDevice, moreComing: Bool)

Tells the delegate that a device has been added.

**Required**

func deviceBrowser(ICDeviceBrowser, didRemove: ICDevice, moreGoing: Bool)

Tells the delegate that a device has been removed.

**Required**

func deviceBrowserDidEnumerateLocalDevices(ICDeviceBrowser)

Tells the delegate that the device browser has completed sending deviceBrowser(_:didAdd:moreComing:) for all local devices.

### Responding to Device Changes

func deviceBrowser(ICDeviceBrowser, requestsSelect: ICDevice)

Tells the delegate when an event occurs on the device that may be of interest to the client application.

func deviceBrowser(ICDeviceBrowser, deviceDidChangeName: ICDevice)

Tells the delegate when the name of a device changes.

func deviceBrowser(ICDeviceBrowser, deviceDidChangeSharingState: ICDevice)

Tells the delegate when the sharing state of a device changes.

### Instance Methods

func deviceBrowserDidCancelSuspendOperations(ICDeviceBrowser)

func deviceBrowserDidResumeOperations(ICDeviceBrowser)

func deviceBrowserDidSuspendOperations(ICDeviceBrowser)

func deviceBrowserWillSuspendOperations(ICDeviceBrowser)

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Managing Device Browsing

var delegate: (any ICDeviceBrowserDelegate)?

The object that acts as the delegate of the device browser.

