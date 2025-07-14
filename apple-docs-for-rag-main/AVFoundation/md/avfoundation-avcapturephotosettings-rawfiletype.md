

- AVFoundation
- AVCapturePhotoSettings
-  rawFileType 

Instance Property

# rawFileType

The container file format for eventual output of the RAW image.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var rawFileType: AVFileType? { get }
```

## Discussion

You specify a file format when creating capture settings with the init(rawPixelFormatType:rawFileType:processedFormat:processedFileType:) initializer. If you didn’t specify a file format, this value is `nil`, and the photo output automatically choosea a default file format appropriate to the rawPhotoPixelFormatType property.

## See Also

### Inspecting settings

var uniqueID: Int64

A unique identifier for this photo settings instance.

var format: [String : Any]?

A dictionary describing the processed format (for example, JPEG) to deliver captured photos in.

var processedFileType: AVFileType?

The container file format for eventual output of the processed image.

var rawPhotoPixelFormatType: OSType

An identifier for the Bayer RAW pixel format to deliver captured RAW photos in.

