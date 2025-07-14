

- AVFoundation
- AVCaptureDevice
-  activeColorSpace 

Instance Property

# activeColorSpace

The currently active color space for capture.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
var activeColorSpace: AVCaptureColorSpace { get set }
```

## Discussion

All devices and formats support capture in the sRGB color space. Some devices and formats can also capture in the P3 color space, which includes a much wider gamut of colors than the sRGB color space. By default, a capture session automatically enables wide-gamut capture for supported devices and capture workflows—for details, see the automaticallyConfiguresCaptureDeviceForWideColor of your capture session. To instead set the color space manually, disable that AVCaptureSession property before setting the active color space.

For best results, choose a color space before calling startRunning() on your capture session. Changing this property while a capture session is running requires a disruptive reconfiguration of the capture render pipeline—movie captures in progress ends immediately, unfulfilled photo requests abort, and video preview temporarily freeze.

Before changing this property, you must call the lockForConfiguration() method to obtain exclusive access to the capture device. Attempting to change this property without locking the device raises an exception (genericException).

## See Also

### Configuring Color Space Settings

enum AVCaptureColorSpace

An enumeration of color spaces a device can support.

