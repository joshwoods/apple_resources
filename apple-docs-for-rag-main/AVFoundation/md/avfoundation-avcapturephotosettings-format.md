

- AVFoundation
- AVCapturePhotoSettings
-  format 

Instance Property

# format

A dictionary describing the processed format (for example, JPEG) to deliver captured photos in.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
var format: [String : Any]? { get }
```

## Discussion

This property is read-only—you specify a processed format when creating a settings object with the photoSettings, init(format:), or init(rawPixelFormatType:processedFormat:) initializer.

When capturing images in processed formats, the following requirements apply:

- This dictionary must contain a value for either the kCVPixelBufferPixelFormatTypeKey (to request an uncompressed format) or AVVideoCodecKey (to request a compressed format such as JPEG) key, but not both.

- If this dictionary has the kCVPixelBufferPixelFormatTypeKey key, the value for that key must be listed in the photo output’s availablePhotoPixelFormatTypes array.

If this dictionary has the AVVideoCodecKey key, the value for that key must be listed in the photo output’s availablePhotoCodecTypes array.

- Your delegate method must implement the photoOutput(_:didFinishProcessingPhoto:previewPhoto:resolvedSettings:bracketSettings:error:) method.

The capture output validates these requirements when you call the capturePhoto(with:delegate:) method. If your settings and delegate do not meet these requirements, that method raises an exception.

## See Also

### Inspecting settings

var uniqueID: Int64

A unique identifier for this photo settings instance.

var processedFileType: AVFileType?

The container file format for eventual output of the processed image.

var rawFileType: AVFileType?

The container file format for eventual output of the RAW image.

var rawPhotoPixelFormatType: OSType

An identifier for the Bayer RAW pixel format to deliver captured RAW photos in.

