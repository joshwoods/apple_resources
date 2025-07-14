

- AVFoundation
- AVCapturePhotoSettings
-  init(rawPixelFormatType:) 

Initializer

# init(rawPixelFormatType:)

Creates a photo settings object for RAW-format-only capture with the specified pixel format.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
convenience init(rawPixelFormatType: OSType)
```

## Parameters 

`rawPixelFormatType`  

The Bayer RAW pixel format type to use for capture. This value must be one of the format identifiers listed in the availableRawPhotoPixelFormatTypes array of your photo capture output.

## Return Value

A new photo settings object.

## Discussion

Use this initializer for RAW-only capture. To capture an image in both RAW format and a processed format (such as JPEG), use the init(rawPixelFormatType:processedFormat:) initializer instead.

Requesting RAW format capture adds requirements for other photo settings: for details, see the rawPhotoPixelFormatType property. The capture output validates these requirements when you call the capturePhoto(with:delegate:) method. If your settings and delegate don’t meet these requirements, that method raises an exception.

## See Also

### Creating photo settings

convenience init(format: [String : Any]?)

Creates a photo settings object with the specified output format.

convenience init(rawPixelFormatType: OSType, processedFormat: [String : Any]?)

Creates a photo settings object for capture in both RAW format and a processed format.

convenience init(rawPixelFormatType: OSType, rawFileType: AVFileType?, processedFormat: [String : Any]?, processedFileType: AVFileType?)

Creates a photo settings object for capture in both RAW format and a processed format with the specified output file types.

convenience init(from: AVCapturePhotoSettings)

Creates a unique photo settings object, copying all settings values from the specified photo settings object.

