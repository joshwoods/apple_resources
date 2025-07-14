

- AVFoundation
- AVPortraitEffectsMatte
-  applyingExifOrientation(\_:) 

Instance Method

# applyingExifOrientation(\_:)

Returns a derivative portrait effects matte after applying the specified EXIF orientation.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func applyingExifOrientation(_ exifOrientation: CGImagePropertyOrientation) -> Self
```

## Parameters 

`exifOrientation`  

One of the standard EXIF orientation tags expressing how the portrait effects matte should be rotated or mirrored.

## See Also

### Creating a Portrait Effects Matte

Configuring Camera Capture to Collect a Portrait Effects Matte

Prepare your app to capture a portrait effects matte when taking photos.

convenience init(fromDictionaryRepresentation: [AnyHashable : Any]) throws

Initializes a portrait effects matte instance from auxiliary image information in an image file.

func replacingPortraitEffectsMatte(with: CVPixelBuffer) throws -> Self

Returns a portrait effects matte by wrapping the replacement pixel buffer.

