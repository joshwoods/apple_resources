

- AVFoundation
- AVCaptureDevice
-  isVideoHDREnabled 

Instance Property

# isVideoHDREnabled

A Boolean value that indicates whether the device streams high dynamic range video buffers, also known as extended dynamic range (EDR).

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var isVideoHDREnabled: Bool { get set }
```

## Discussion

The device ignores the value of this property when activeColorSpace is HLG BT2020 color space because HDR is effectively always on and can’t be disabled.

Before changing the value of this property, you must call lockForConfiguration() to acquire exclusive access to the device’s configuration properties. Otherwise, setting the value of this property raises an exception. When you finish configuring the device, call unlockForConfiguration() to release the lock and allow other devices to configure the settings.

Note that setting this property may cause a lengthy reconfiguration of the device, similar to setting a new active format or capture session preset. If you’re setting either the active format or the sessionPreset *and* this property, you should bracket these operations with beginConfiguration() and session commitConfiguration() to minimize reconfiguration time.

This property is key-value observable.

## See Also

### Configuring HDR Settings

var automaticallyAdjustsVideoHDREnabled: Bool

A Boolean value that indicates whether the device automatically manages the state of high dynamic range (HDR) video streaming.

