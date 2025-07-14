

- AVFoundation
- AVCapturePhotoSettings
-  init(from:) 

Initializer

# init(from:)

Creates a unique photo settings object, copying all settings values from the specified photo settings object.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
convenience init(from photoSettings: AVCapturePhotoSettings)
```

## Parameters 

`photoSettings`  

The photo settings object from which to copy settings.

## Return Value

A new photo settings object.

## Discussion

It is illegal to reuse a AVCapturePhotoSettings instance for multiple captures. Calling the capturePhoto(with:delegate:) method throws an exception if the uniqueID value of the `settings` parameter matches that of any previously used settings object.

To reuse a specific combination of settings, use this initializer to create a new AVCapturePhotoSettings instance from an existing photo settings object. The newly created instance has a new, unique value for its uniqueID property, but copies the values for all other properties from the `photoSettings` parameter.

## See Also

### Creating photo settings

convenience init(format: [String : Any]?)

Creates a photo settings object with the specified output format.

convenience init(rawPixelFormatType: OSType)

Creates a photo settings object for RAW-format-only capture with the specified pixel format.

convenience init(rawPixelFormatType: OSType, processedFormat: [String : Any]?)

Creates a photo settings object for capture in both RAW format and a processed format.

convenience init(rawPixelFormatType: OSType, rawFileType: AVFileType?, processedFormat: [String : Any]?, processedFileType: AVFileType?)

Creates a photo settings object for capture in both RAW format and a processed format with the specified output file types.

