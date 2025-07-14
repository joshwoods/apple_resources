

- AVFoundation
- AVPortraitEffectsMatte
-  replacingPortraitEffectsMatte(with:) 

Instance Method

# replacingPortraitEffectsMatte(with:)

Returns a portrait effects matte by wrapping the replacement pixel buffer.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func replacingPortraitEffectsMatte(with pixelBuffer: CVPixelBuffer) throws -> Self
```

## Parameters 

`pixelBuffer`  

A pixel buffer containing a portrait effects matte image, represented as kCVPixelFormatType_OneComponent8 with kCVImageBufferColorPrimaries_ITU_R_709_2 color primaries and a kCVImageBufferTransferFunction_Linear transfer function.

## See Also

### Creating a Portrait Effects Matte

Configuring Camera Capture to Collect a Portrait Effects Matte

Prepare your app to capture a portrait effects matte when taking photos.

convenience init(fromDictionaryRepresentation: [AnyHashable : Any]) throws

Initializes a portrait effects matte instance from auxiliary image information in an image file.

func applyingExifOrientation(CGImagePropertyOrientation) -> Self

Returns a derivative portrait effects matte after applying the specified EXIF orientation.

