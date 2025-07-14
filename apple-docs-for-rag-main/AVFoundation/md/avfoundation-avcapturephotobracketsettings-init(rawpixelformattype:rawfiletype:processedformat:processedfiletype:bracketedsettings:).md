

- AVFoundation
- AVCapturePhotoBracketSettings
-  init(rawPixelFormatType:rawFileType:processedFormat:processedFileType:bracketedSettings:) 

Initializer

# init(rawPixelFormatType:rawFileType:processedFormat:processedFileType:bracketedSettings:)

Creates a photo settings object for capture in both RAW format and a processed format.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
convenience init(
    rawPixelFormatType: OSType,
    rawFileType: AVFileType?,
    processedFormat: [String : Any]?,
    processedFileType: AVFileType?,
    bracketedSettings: [AVCaptureBracketedStillImageSettings]
)
```

## Parameters 

`rawPixelFormatType`  

The Bayer RAW pixel format type to use for capture. This value must be one of the format identifiers listed in the availableRawPhotoPixelFormatTypes array of your photo capture output.

`rawFileType`  

The container file format for eventual output of the RAW image.

If you have no preferred file format, pass `nil` and the photo output will automatically choose a default file format appropriate to the `rawPixelFormatType` parameter.

`processedFormat`  

A dictionary of Core Video pixel buffer attributes or AVFoundation video settings constants (see `Video Settings`).

To capture a photo in an uncompressed format, such as 420f, 420v, or BGRA, set the key kCVPixelBufferPixelFormatTypeKey in the `format` dictionary. The corresponding value must be one of the pixel format identifiers listed in the availablePhotoPixelFormatTypes array of your photo capture output.

To capture a photo in a compressed format, such as JPEG, set the key AVVideoCodecKey in the `format` dictionary. The corresponding value must be one of the codec identifiers listed in the availablePhotoCodecTypes array of your photo capture output. For a compressed format, you can also specify a compression level with the key AVVideoQualityKey.

`processedFileType`  

The container file format for eventual output of the processed image.

If you have no preferred file format, pass `nil` and the photo output will automatically choose a default file format appropriate to the `processedFormat` parameter.

`bracketedSettings`  

An array of either AVCaptureManualExposureBracketedStillImageSettings or AVCaptureAutoExposureBracketedStillImageSettings objects, each of which describes the variation in camera settings to use for one image in the bracketed capture.

The number of image settings objects in this array must be greater than zero and less than or equal to the maxBracketedCapturePhotoCount value of your photo output. All image settings objects in this array must be the same type. Calling this initializer with an invalid number or combination of image settings objects raises an exception (invalidArgumentException).

## Return Value

A new photo settings object.

## Discussion

Use this initializer to capture an image in both RAW format and a processed format (such as JPEG). For RAW-only capture, use the init(rawPixelFormatType:) initializer instead.

Requesting both formats adds requirements for other photo settings: see the format property for processed format requirements and the rawPhotoPixelFormatType property for RAW format requirements. The capture output validates these requirements when you call the capturePhoto(with:delegate:) method. If your settings and delegate do not meet these requirements, that method raises an exception.

## See Also

### Creating a Bracket Settings Object

convenience init(rawPixelFormatType: OSType, processedFormat: [String : Any]?, bracketedSettings: [AVCaptureBracketedStillImageSettings])

Creates a photo settings object for the specified bracket of captures, in the specified formats.

