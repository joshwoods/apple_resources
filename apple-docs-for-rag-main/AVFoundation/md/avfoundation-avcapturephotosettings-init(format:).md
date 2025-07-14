

- AVFoundation
- AVCapturePhotoSettings
-  init(format:) 

Initializer

# init(format:)

Creates a photo settings object with the specified output format.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
convenience init(format: [String : Any]?)
```

## Parameters 

`format`  

A dictionary of Core Video pixel buffer attributes or AVFoundation video settings constants (see Video Settings).

To capture a photo in an uncompressed format, such as 420f, 420v, or BGRA, set the key kCVPixelBufferPixelFormatTypeKey in the `format` dictionary. The corresponding value must be one of the pixel format identifiers listed in the availablePhotoPixelFormatTypes array of your photo capture output.

To capture a photo in a compressed format, such as JPEG, set the key AVVideoCodecKey in the `format` dictionary. The corresponding value must be one of the codec identifiers listed in the availablePhotoCodecTypes array of your photo capture output. For a compressed format, you can also specify a compression level with the key AVVideoQualityKey.

## Return Value

A new photo settings object.

## Mentioned in 

Capturing Uncompressed Image Data

## Discussion

Requesting capture in a processed format adds requirements for other photo settings: for details, see the format property. The capture output validates these requirements when you call the capturePhoto(with:delegate:) method. If your settings and delegate don’t meet these requirements, that method raises an exception.

## See Also

### Creating photo settings

convenience init(rawPixelFormatType: OSType)

Creates a photo settings object for RAW-format-only capture with the specified pixel format.

convenience init(rawPixelFormatType: OSType, processedFormat: [String : Any]?)

Creates a photo settings object for capture in both RAW format and a processed format.

convenience init(rawPixelFormatType: OSType, rawFileType: AVFileType?, processedFormat: [String : Any]?, processedFileType: AVFileType?)

Creates a photo settings object for capture in both RAW format and a processed format with the specified output file types.

convenience init(from: AVCapturePhotoSettings)

Creates a unique photo settings object, copying all settings values from the specified photo settings object.

