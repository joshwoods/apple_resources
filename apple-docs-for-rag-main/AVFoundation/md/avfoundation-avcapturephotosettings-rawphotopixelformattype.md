

- AVFoundation
- AVCapturePhotoSettings
-  rawPhotoPixelFormatType 

Instance Property

# rawPhotoPixelFormatType

An identifier for the Bayer RAW pixel format to deliver captured RAW photos in.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var rawPhotoPixelFormatType: OSType { get }
```

## Discussion

This property is read-only—you specify a RAW pixel format when creating a settings object with the init(rawPixelFormatType:), init(rawPixelFormatType:processedFormat:) initializer.

When capturing RAW images, the following requirements apply:

- The isAutoStillImageStabilizationEnabled setting must be false.

- Your delegate object must implement the photoOutput(_:didFinishProcessingRawPhoto:previewPhoto:resolvedSettings:bracketSettings:error:) method.

- The isHighResolutionPhotoEnabled setting may be true or false, but that setting applies only to the separate processed image.

(You request separate processed images with the init(rawPixelFormatType:processedFormat:) initializer. This restriction does not apply when you request RAW-only capture with the init(rawPixelFormatType:) initializer).

The capture output validates these requirements when you call the capturePhoto(with:delegate:) method. If your settings and delegate do not meet these requirements, that method raises an exception.

## See Also

### Inspecting settings

var uniqueID: Int64

A unique identifier for this photo settings instance.

var format: [String : Any]?

A dictionary describing the processed format (for example, JPEG) to deliver captured photos in.

var processedFileType: AVFileType?

The container file format for eventual output of the processed image.

var rawFileType: AVFileType?

The container file format for eventual output of the RAW image.

