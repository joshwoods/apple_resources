

- AVFoundation
- AVCapturePhotoFileDataRepresentationCustomizer
-  replacementPortraitEffectsMatte(for:) 

Instance Method

# replacementPortraitEffectsMatte(for:)

A callback in which you can provide a replacement portrait effects matte, or strip the existing portrait effects matte from the file.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
optional func replacementPortraitEffectsMatte(for photo: AVCapturePhoto) -> AVPortraitEffectsMatte?
```

## Parameters 

`photo`  

The calling instance of AVCapturePhoto whose file metadata you’re modifying.

## Return Value

An instance of AVPortraitEffectsMatte. To preserve the existing portrait effects matte, return `photo.portraitEffectsMatte`. To strip the existing portrait effects matte, return `nil`. To replace the portrait effects matte, provide a replacement AVPortraitEffectsMatte instance.

## Discussion

This callback is optional. If your delegate doesn’t implement this callback, the existing metadata in the in-memory AVCapturePhoto container is written directly to the file data representation.

## See Also

### Replacing or Removing Metadata

func replacementMetadata(for: AVCapturePhoto) -> [String : Any]?

A callback in which you can provide replacement metadata or direct AVCapturePhoto to strip existing metadata from the flattened file.

func replacementEmbeddedThumbnailPixelBuffer(withPhotoFormat: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>, for: AVCapturePhoto) -> Unmanaged&lt;CVPixelBuffer>?

A callback in which you can provide a replacement embedded thumbnail image with compression settings, or strip the existing embedded thumbnail image from the flattened file.

func replacementDepthData(for: AVCapturePhoto) -> AVDepthData?

A callback in which you can provide replacement depth data or strip existing depth data from the file.

func replacementSemanticSegmentationMatte(ofType: AVSemanticSegmentationMatte.MatteType, for: AVCapturePhoto) -> AVSemanticSegmentationMatte?

Replaces or removes the semantic segmentation matte of the specified type from the flattened file data representation.

func replacementAppleProRAWCompressionSettings(for: AVCapturePhoto, defaultSettings: [String : Any], maximumBitDepth: Int) -> [String : Any]

Replaces the compression settings the system uses when writing Apple ProRAW data to a Linear DNG file.

