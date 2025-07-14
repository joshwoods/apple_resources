

- AVFoundation
- AVCapturePhotoSettings
-  init(rawPixelFormatType:processedFormat:) 

Initializer

# init(rawPixelFormatType:processedFormat:)

Creates a photo settings object for capture in both RAW format and a processed format.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
convenience init(
    rawPixelFormatType: OSType,
    processedFormat: [String : Any]?
)
```

## Parameters 

`rawPixelFormatType`  

The Bayer RAW pixel format type to use for capture. This value must be one of the format identifiers listed in the availableRawPhotoPixelFormatTypes array of your photo capture output.

`processedFormat`  

A dictionary of Core Video pixel buffer attributes or AVFoundation video settings constants (see `Video Settings`).

To capture a photo in an uncompressed format, such as 420f, 420v, or BGRA, set the key kCVPixelBufferPixelFormatTypeKey in the `format` dictionary. The corresponding value must be one of the pixel format identifiers listed in the availablePhotoPixelFormatTypes array of your photo capture output.

To capture a photo in a compressed format, such as JPEG, set the key AVVideoCodecKey in the `format` dictionary. The corresponding value must be one of the codec identifiers listed in the availablePhotoCodecTypes array of your photo capture output. For a compressed format, you can also specify a compression level with the key AVVideoQualityKey.

## Return Value

A new photo settings object.

## Discussion

Use this initializer to capture an image in both RAW format and a processed format (such as JPEG). For RAW-only capture, use the init(rawPixelFormatType:) initializer instead.

Requesting both formats adds requirements for other photo settings: see the format property for processed format requirements and the rawPhotoPixelFormatType property for RAW format requirements. The capture output validates these requirements when you call the capturePhoto(with:delegate:) method. If your settings and delegate don’t meet these requirements, that method raises an exception.

## See Also

### Creating photo settings

convenience init(format: [String : Any]?)

Creates a photo settings object with the specified output format.

convenience init(rawPixelFormatType: OSType)

Creates a photo settings object for RAW-format-only capture with the specified pixel format.

convenience init(rawPixelFormatType: OSType, rawFileType: AVFileType?, processedFormat: [String : Any]?, processedFileType: AVFileType?)

Creates a photo settings object for capture in both RAW format and a processed format with the specified output file types.

convenience init(from: AVCapturePhotoSettings)

Creates a unique photo settings object, copying all settings values from the specified photo settings object.

