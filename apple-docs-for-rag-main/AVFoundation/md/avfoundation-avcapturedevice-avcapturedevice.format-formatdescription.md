

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  formatDescription 

Instance Property

# formatDescription

An object describing the capture format.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
var formatDescription: CMFormatDescription { get }
```

## Discussion

Calling this method doesn’t assume ownership of the returned CMFormatDescription.

## See Also

### Determining Supported Media Formats

var mediaType: AVMediaType

A constant describing the media type of an `AVCaptureDevice` active or supported format.

