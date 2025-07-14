

- AVFoundation
- AVCapturePhotoOutput
-  availableRawPhotoPixelFormatTypes 

Instance Property

# availableRawPhotoPixelFormatTypes

The pixel formats the capture output supports for RAW photo capture.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 11.0+tvOS 17.0+

``` source
@nonobjc
var availableRawPhotoPixelFormatTypes: [OSType] { get }
```

## Discussion

To capture a photo in RAW format, use the init(rawPixelFormatType:) or init(rawPixelFormatType:processedFormat:) initializer to create your photo settings object. The value for that initializer’s `rawPixelFormatType` parameter must be one of the Bayer RAW format identifiers listed in this array.

Note

Read this property only after adding the photo capture output to an AVCaptureSession object containing a video source. If the photo capture output isn’t connected to a session with a video source, this array is empty.

Not all devices support RAW image capture. If the current device doesn’t support RAW capture, this array is empty.

This property supports key-value observing.

## See Also

### Determining Supported Pixel Formats

var availablePhotoPixelFormatTypes: [OSType]

The pixel formats the capture output supports for photo capture.

func supportedPhotoPixelFormatTypes(for: AVFileType) -> [OSType]

Returns the list of uncompressed pixel formats supported for photo data in the specified file type.

func supportedRawPhotoPixelFormatTypes(for: AVFileType) -> [OSType]

Returns the list of Bayer RAW pixel formats supported for photo data in the specified file type.

class func isAppleProRAWPixelFormat(OSType) -> Bool

Returns a Boolean value that indicates whether the pixel format is an Apple ProRAW format.

class func isBayerRAWPixelFormat(OSType) -> Bool

Returns a Boolean value that indicates whether the pixel format is a Bayer RAW format.

