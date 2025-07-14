

- AVFoundation
- AVCapturePhotoFileDataRepresentationCustomizer
-  replacementEmbeddedThumbnailPixelBuffer(withPhotoFormat:for:) 

Instance Method

# replacementEmbeddedThumbnailPixelBuffer(withPhotoFormat:for:)

A callback in which you can provide a replacement embedded thumbnail image with compression settings, or strip the existing embedded thumbnail image from the flattened file.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
optional func replacementEmbeddedThumbnailPixelBuffer(
    withPhotoFormat replacementEmbeddedThumbnailPhotoFormatOut: AutoreleasingUnsafeMutablePointer,
    for photo: AVCapturePhoto
) -> Unmanaged?
```

## Parameters 

`replacementEmbeddedThumbnailPhotoFormatOut`  

A pointer to a dictionary of keys and values from `AVFoundation/AVVideoSettings.h`. If you pass a non-nil dictionary, AVVideoCodecKey is required, with `width` and `height` keys optional.

`photo`  

The calling instance of AVCapturePhoto whose file metadata you’re modifying.

## Return Value

A pixel buffer containing a source image to be encoded to the file as the replacement thumbnail image. To preserve the existing embedded thumbnail photo to the flattened data, set `replacementEmbeddedThumbnailPhotoFormatOut` to `photo.embeddedThumbnailPhotoFormat` and return `nil`. To replace the existing embedded thumbnail, pass a replacement photo format dictionary and return a non-`nil` replacement pixel buffer. To remove the existing embedded thumbnail, set `replacementEmbeddedThumbnailPhotoFormatOut` to `nil` and return `nil`.

## Discussion

This callback is optional. If your delegate doesn’t implement this callback, the existing metadata in the in-memory AVCapturePhoto container is written directly to the file data representation.

## See Also

### Replacing or Removing Metadata

func replacementMetadata(for: AVCapturePhoto) -> [String : Any]?

A callback in which you can provide replacement metadata or direct AVCapturePhoto to strip existing metadata from the flattened file.

func replacementDepthData(for: AVCapturePhoto) -> AVDepthData?

A callback in which you can provide replacement depth data or strip existing depth data from the file.

func replacementPortraitEffectsMatte(for: AVCapturePhoto) -> AVPortraitEffectsMatte?

A callback in which you can provide a replacement portrait effects matte, or strip the existing portrait effects matte from the file.

func replacementSemanticSegmentationMatte(ofType: AVSemanticSegmentationMatte.MatteType, for: AVCapturePhoto) -> AVSemanticSegmentationMatte?

Replaces or removes the semantic segmentation matte of the specified type from the flattened file data representation.

func replacementAppleProRAWCompressionSettings(for: AVCapturePhoto, defaultSettings: [String : Any], maximumBitDepth: Int) -> [String : Any]

Replaces the compression settings the system uses when writing Apple ProRAW data to a Linear DNG file.

