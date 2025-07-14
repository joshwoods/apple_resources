

- AVFoundation
- AVCapturePhotoOutput
-  isBayerRAWPixelFormat(\_:) 

Type Method

# isBayerRAWPixelFormat(\_:)

Returns a Boolean value that indicates whether the pixel format is a Bayer RAW format.

iOS 14.3+iPadOS 14.3+Mac Catalyst 14.3+tvOS 17.0+

``` source
class func isBayerRAWPixelFormat(_ pixelFormat: OSType) -> Bool
```

## Parameters 

`pixelFormat`  

The pixel format to query.

## Return Value

true if the pixel format is a Bayer RAW format, otherwise false.

## Mentioned in 

Capturing Photos in RAW and Apple ProRAW Formats

## See Also

### Determining Supported Pixel Formats

var availablePhotoPixelFormatTypes: [OSType]

The pixel formats the capture output supports for photo capture.

var availableRawPhotoPixelFormatTypes: [OSType]

The pixel formats the capture output supports for RAW photo capture.

func supportedPhotoPixelFormatTypes(for: AVFileType) -> [OSType]

Returns the list of uncompressed pixel formats supported for photo data in the specified file type.

func supportedRawPhotoPixelFormatTypes(for: AVFileType) -> [OSType]

Returns the list of Bayer RAW pixel formats supported for photo data in the specified file type.

class func isAppleProRAWPixelFormat(OSType) -> Bool

Returns a Boolean value that indicates whether the pixel format is an Apple ProRAW format.

