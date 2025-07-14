

- AVFoundation
- AVCapturePhotoSettings
-  uniqueID 

Instance Property

# uniqueID

A unique identifier for this photo settings instance.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
var uniqueID: Int64 { get }
```

## Mentioned in 

Tracking Photo Capture Progress

## Discussion

Creating a AVCapturePhotoSettings instance automatically assigns a unique value to this property.

Use this property to track a photo capture request. After you call the capturePhoto(with:delegate:) method, the photo capture output calls your delegate object to provide information about the progress and results of the capture. Each delegate method includes a AVCaptureResolvedPhotoSettings whose uniqueID property matches the uniqueID value of the AVCapturePhotoSettings object you used to request capture.

It is illegal to reuse a AVCapturePhotoSettings instance for multiple captures. Calling the capturePhoto(with:delegate:) method throws an exception (invalidArgumentException) if the `settings` object’s uniqueID value matches that of any previously used settings object.

## See Also

### Inspecting settings

var format: [String : Any]?

A dictionary describing the processed format (for example, JPEG) to deliver captured photos in.

var processedFileType: AVFileType?

The container file format for eventual output of the processed image.

var rawFileType: AVFileType?

The container file format for eventual output of the RAW image.

var rawPhotoPixelFormatType: OSType

An identifier for the Bayer RAW pixel format to deliver captured RAW photos in.

