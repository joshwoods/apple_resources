

- AVFoundation
- AVCapturePhotoOutput
-  supportedPhotoPixelFormatTypes(for:) 

Instance Method

# supportedPhotoPixelFormatTypes(for:)

Returns the list of uncompressed pixel formats supported for photo data in the specified file type.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
@nonobjc
func supportedPhotoPixelFormatTypes(for fileType: AVFileType) -> [OSType]
```

## Parameters 

`fileType`  

The file type for which to obtain format information.

## Return Value

An array of pixel format types supported for encoding in the specified file type.

## Discussion

When you issue a photo capture request, you can separately specify the format for capturing or encoding image data and the container format for producing output files containing that data. However, each file type supports only a specific set of image data types.

After choosing a file type from the availablePhotoFileTypes array, use this method to find a compatible image data format before creating a photo settings object.

## See Also

### Determining Supported Pixel Formats

var availablePhotoPixelFormatTypes: [OSType]

The pixel formats the capture output supports for photo capture.

var availableRawPhotoPixelFormatTypes: [OSType]

The pixel formats the capture output supports for RAW photo capture.

func supportedRawPhotoPixelFormatTypes(for: AVFileType) -> [OSType]

Returns the list of Bayer RAW pixel formats supported for photo data in the specified file type.

class func isAppleProRAWPixelFormat(OSType) -> Bool

Returns a Boolean value that indicates whether the pixel format is an Apple ProRAW format.

class func isBayerRAWPixelFormat(OSType) -> Bool

Returns a Boolean value that indicates whether the pixel format is a Bayer RAW format.

