

- ImageCaptureCore
- ICCameraDevice
-  isEjectable 

Instance Property

# isEjectable

A Boolean value indicating whether the device can be ‘soft’ removed or disconnected.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
var isEjectable: Bool { get }
```

## Discussion

Soft ejecting an SD card is equivalent to unmounting it in Finder without physically removing it from the host.

