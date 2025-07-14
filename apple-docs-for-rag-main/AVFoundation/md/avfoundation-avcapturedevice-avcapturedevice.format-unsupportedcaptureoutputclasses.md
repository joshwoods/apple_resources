

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  unsupportedCaptureOutputClasses 

Instance Property

# unsupportedCaptureOutputClasses

The list of capture output subclasses not allowed for capture with this format, if any.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var unsupportedCaptureOutputClasses: [AnyClass] { get }
```

## Discussion

As a rule, capture formats with a given mediaType are available for use with all AVCaptureOutput subclasses that accept that media type. However, this isn’t always the case. For example, formats for high-resolution photo capture may not support the AVCaptureMovieFileOutput class due to bandwidth limitations.

