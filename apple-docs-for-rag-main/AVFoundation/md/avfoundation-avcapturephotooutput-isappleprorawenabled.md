

- AVFoundation
- AVCapturePhotoOutput
-  isAppleProRAWEnabled 

Instance Property

# isAppleProRAWEnabled

A Boolean value that indicates whether you’ve configured the photo output to deliver Apple ProRAW formats.

iOS 14.3+iPadOS 14.3+Mac Catalyst 14.3+tvOS 17.0+

``` source
var isAppleProRAWEnabled: Bool { get set }
```

## Mentioned in 

Capturing Photos in RAW and Apple ProRAW Formats

## Discussion

If isAppleProRAWSupported returns true, you can enable Apple ProRAW capture by setting this property to true. Compared to photos taken in Bayer RAW format, the system demosaics and partially processes Apple ProRAW photos. They’re still scene-referred, however, and allow capturing RAW photos in modes that don’t have a traditional Bayer RAW format available, such as modes that rely on fusing multiple captures.

Apple ProRAW formats aren’t supported on all platforms and devices. You can determine the pixel formats the system supports by querying the availableRawPhotoPixelFormatTypes property. Use the isBayerRAWPixelFormat(_:) or isAppleProRAWPixelFormat(_:) method to determine whether the pixel format is Bayer RAW or Apple ProRAW, respectively.

This property is key-value observable.

Tip

Set this property to true before calling startRunning() on the capture session. Enabling this property later requires a lengthy reconfiguration of the capture pipeline.

## See Also

### Configuring ProRAW Support

var isAppleProRAWSupported: Bool

A Boolean value that indicates whether the current device and configuration supports Apple ProRAW pixel formats.

