

- AVFoundation
- AVPortraitEffectsMatte
-  init(fromDictionaryRepresentation:) 

Initializer

# init(fromDictionaryRepresentation:)

Initializes a portrait effects matte instance from auxiliary image information in an image file.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
convenience init(fromDictionaryRepresentation imageSourceAuxDataInfoDictionary: [AnyHashable : Any]) throws
```

## Parameters 

`imageSourceAuxDataInfoDictionary`  

A dictionary of information related to primitive portrait effects matte; obtained from CGImageSourceCopyAuxiliaryDataInfoAtIndex(_:_:_:).

## Mentioned in 

Extracting Portrait Effects Matte Image Data from a Photo

## Discussion

When using the Image I/O API to read from a HEIF or JPEG file containing a portrait effects matte, you can create an AVPortraitEffectsMatte object from the result of CGImageSourceCopyAuxiliaryDataInfoAtIndex(_:_:_:). This function returns a CFDictionary of primitive map information.

## See Also

### Creating a Portrait Effects Matte

Configuring Camera Capture to Collect a Portrait Effects Matte

Prepare your app to capture a portrait effects matte when taking photos.

func applyingExifOrientation(CGImagePropertyOrientation) -> Self

Returns a derivative portrait effects matte after applying the specified EXIF orientation.

func replacingPortraitEffectsMatte(with: CVPixelBuffer) throws -> Self

Returns a portrait effects matte by wrapping the replacement pixel buffer.

