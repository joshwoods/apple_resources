

- AVFoundation
- AVCaptureDevice
-  automaticallyAdjustsVideoHDREnabled 

Instance Property

# automaticallyAdjustsVideoHDREnabled

A Boolean value that indicates whether the device automatically manages the state of high dynamic range (HDR) video streaming.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var automaticallyAdjustsVideoHDREnabled: Bool { get set }
```

## Discussion

By default, this value is `true`, and a capture device automatically enables isVideoHDREnabled if it’s a good fit for the active format.

This property is key-value observable.

## See Also

### Configuring HDR Settings

var isVideoHDREnabled: Bool

A Boolean value that indicates whether the device streams high dynamic range video buffers, also known as extended dynamic range (EDR).

