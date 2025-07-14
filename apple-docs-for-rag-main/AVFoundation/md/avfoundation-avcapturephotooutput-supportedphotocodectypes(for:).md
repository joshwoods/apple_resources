

- AVFoundation
- AVCapturePhotoOutput
-  supportedPhotoCodecTypes(for:) 

Instance Method

# supportedPhotoCodecTypes(for:)

Returns the list of photo codecs (such as JPEG or HEVC) supported for photo data in the specified file type.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
func supportedPhotoCodecTypes(for fileType: AVFileType) -> [AVVideoCodecType]
```

## Parameters 

`fileType`  

The file type (such as JFIF or HEIF) for which to obtain codec information.

## Return Value

An array of video codec types supported for encoding in the specified file type.

## Discussion

When you issue a photo capture request, you can separately specify the format for capturing or encoding image data and the container format for producing output files containing that data. However, each file type supports only a specific set of image data types.

After choosing a file type from the availablePhotoFileTypes array, use this method to find a compatible image data codec before creating a photo settings object.

## See Also

### Determining Supported Codec Types

var availablePhotoCodecTypes: [AVVideoCodecType]

The compression codecs this capture output currently supports for photo capture.

