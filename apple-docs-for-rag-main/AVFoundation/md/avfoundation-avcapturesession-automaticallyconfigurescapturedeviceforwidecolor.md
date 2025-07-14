

- AVFoundation
- AVCaptureSession
-  automaticallyConfiguresCaptureDeviceForWideColor 

Instance Property

# automaticallyConfiguresCaptureDeviceForWideColor

A Boolean value that specifies whether the session should automatically use wide-gamut color where available.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var automaticallyConfiguresCaptureDeviceForWideColor: Bool { get set }
```

## Discussion

All devices and formats support capture in the sRGB color space. Some devices and formats can also capture in the P3 color space, which includes a much wider gamut of colors. Wide-gamut capture is appropriate for only certain capture workflows, so this property controls automatic configuration for those workflows.

When this property is true (the default), and your session configuration is appropriate for wide-gamut capture:

- If you use a session preset other than inputPriority, the session automatically sets the device’s activeFormat property to one that supports wide-gamut capture, and sets the device’s activeColorSpace property to a wide-gamut color space.

- If you manually choose a capture format (thereby setting the session to input priority), the session automatically sets the device’s activeColorSpace property to a wide-gamut color space only if your chosen format supports wide-gamut capture.

For information about which devices and session configurations automatically enable wide-gamut capture, see Wide-Gamut Capture in iOS Device Compatibility Reference.

Note

When this property is true, and your session configuration isn’t appropriate for wide-gamut capture, session presets other than inputPriority may choose a capture format that doesn’t support wide-gamut capture.

Set this property to false if you want to directly change the value of the capture device’s activeColorSpace property (regardless of whether you configure your device with a session preset or by directly setting a capture format).

