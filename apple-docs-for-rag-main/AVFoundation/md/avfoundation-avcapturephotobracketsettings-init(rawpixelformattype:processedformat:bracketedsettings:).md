

- AVFoundation
- AVCapturePhotoBracketSettings
-  init(rawPixelFormatType:processedFormat:bracketedSettings:) 

Initializer

# init(rawPixelFormatType:processedFormat:bracketedSettings:)

Creates a photo settings object for the specified bracket of captures, in the specified formats.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
convenience init(
    rawPixelFormatType: OSType,
    processedFormat: [String : Any]?,
    bracketedSettings: [AVCaptureBracketedStillImageSettings]
)
```

## Parameters 

`rawPixelFormatType`  

The pixel format type for capture in a Bayer RAW format. This value must be one of the format identifiers listed in the availableRawPhotoPixelFormatTypes array of your photo capture output.

`processedFormat`  

A dictionary of Core Video pixel buffer attributes or AVFoundation video settings constants (see `Video Settings`) for capturing images in a processed format.

To capture a photo in an uncompressed format, such as 420f, 420v, or BGRA, set the key kCVPixelBufferPixelFormatTypeKey in the format dictionary. The corresponding value must be one of the pixel format identifiers listed in the availablePhotoPixelFormatTypes array of your photo capture output.

To capture a photo in a compressed format, such as JPEG, set the key AVVideoCodecKey in the format dictionary. The corresponding value must be one of the codec identifiers listed in the availablePhotoCodecTypes array of your photo capture output. For a compressed format, you can also specify a compression level with the key AVVideoQualityKey.

`bracketedSettings`  

An array of either AVCaptureManualExposureBracketedStillImageSettings or AVCaptureAutoExposureBracketedStillImageSettings objects, each of which describes the variation in camera settings to use for one image in the bracketed capture.

The number of image settings objects in this array must be greater than zero and less than or equal to the maxBracketedCapturePhotoCount value of your photo output. All image settings objects in this array must be the same type. Calling this initializer with an invalid number or combination of image settings objects raises an exception (invalidArgumentException).

## Return Value

A new photo settings object.

## Discussion

To request bracketed image capture, create an array of AVCaptureBracketedStillImageSettings objects, each of which describes a variation in capture settings to use for one exposure in the bracket, and pass that array for the `bracketedSettings` parameter. The number of bracketed settings objects in that array determines the number of exposures in the capture bracket.

To capture only in RAW format, pass `nil` for the `processedFormat` parameter. To capture only in a processed format, pass zero for the `rawPixelFormatType` parameter. Passing both `nil` for the `processedFormat` parameter and zero for the `rawPixelFormatType` parameter is equivalent to requesting JPEG-only delivery.

Requesting either or both formats adds requirements for other photo settings: see the format property for processed format requirements and the rawPhotoPixelFormatType property for RAW format requirements. Additionally, the number of still image settings objects in this array must be no greater than the maxBracketedCapturePhotoCount value of your photo output. The capture output validates these requirements when you call the capturePhoto(with:delegate:) method. If your your settings and delegate do not meet these requirements, that method raises an exception.

## See Also

### Creating a Bracket Settings Object

convenience init(rawPixelFormatType: OSType, rawFileType: AVFileType?, processedFormat: [String : Any]?, processedFileType: AVFileType?, bracketedSettings: [AVCaptureBracketedStillImageSettings])

Creates a photo settings object for capture in both RAW format and a processed format.

