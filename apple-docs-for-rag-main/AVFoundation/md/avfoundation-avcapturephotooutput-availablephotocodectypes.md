

- AVFoundation
- AVCapturePhotoOutput
-  availablePhotoCodecTypes 

Instance Property

# availablePhotoCodecTypes

The compression codecs this capture output currently supports for photo capture.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
var availablePhotoCodecTypes: [AVVideoCodecType] { get }
```

## Discussion

To capture a photo in a compressed format, such as JPEG, use the init(format:) initializer to create your photo settings object. In that initializer’s `format` dictionary, pass the key AVVideoCodecKey, whose value must be one of the codec identifiers listed in this array.

Note

Read this property only after adding the photo capture output to an AVCaptureSession object containing a video source. If the photo capture output isn’t connected to a session with a video source, this array is empty.

This property supports key-value observing.

## See Also

### Determining Supported Codec Types

func supportedPhotoCodecTypes(for: AVFileType) -> [AVVideoCodecType]

Returns the list of photo codecs (such as JPEG or HEVC) supported for photo data in the specified file type.

