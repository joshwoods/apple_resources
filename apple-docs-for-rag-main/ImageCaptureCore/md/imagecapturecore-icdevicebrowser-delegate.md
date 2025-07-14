

- ImageCaptureCore
- ICDeviceBrowser
-  delegate 

Instance Property

# delegate

The object that acts as the delegate of the device browser.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
unowned(unsafe) var delegate: (any ICDeviceBrowserDelegate)? { get set }
```

## See Also

### Managing Device Browsing

protocol ICDeviceBrowserDelegate

Methods for managing the addition and removal of devices and responding to device changes.

