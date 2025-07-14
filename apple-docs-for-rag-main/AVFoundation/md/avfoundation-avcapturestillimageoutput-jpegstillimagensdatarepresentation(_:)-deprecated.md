

- AVFoundation
- AVCaptureStillImageOutput
-  jpegStillImageNSDataRepresentation(\_:) Deprecated

Type Method

# jpegStillImageNSDataRepresentation(\_:)

Returns an `NSData` representation of a still image data and metadata attachments in a JPEG sample buffer.

iOS 4.0–10.0DeprecatediPadOS 4.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.7–10.15Deprecated

``` source
class func jpegStillImageNSDataRepresentation(_ jpegSampleBuffer: CMSampleBuffer) -> Data?
```

Deprecated

Use AVCapturePhotoOutput instead.

## Parameters 

`jpegSampleBuffer`  

The sample buffer carrying JPEG image data, optionally with `Exif` metadata sample buffer attachments.

This method throws an invalidArgumentException if `jpegSampleBuffer` is `NULL` or not in the JPEG format.

## Return Value

An `NSData` representation of `jpegSampleBuffer`.

## Discussion

This method merges the image data and `Exif` metadata sample buffer attachments without recompressing the image.

The returned `NSData` object is suitable for writing to disk.

