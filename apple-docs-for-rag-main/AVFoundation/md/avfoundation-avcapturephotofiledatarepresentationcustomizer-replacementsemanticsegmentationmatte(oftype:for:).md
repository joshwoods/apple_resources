

- AVFoundation
- AVCapturePhotoFileDataRepresentationCustomizer
-  replacementSemanticSegmentationMatte(ofType:for:) 

Instance Method

# replacementSemanticSegmentationMatte(ofType:for:)

Replaces or removes the semantic segmentation matte of the specified type from the flattened file data representation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
optional func replacementSemanticSegmentationMatte(
    ofType semanticSegmentationMatteType: AVSemanticSegmentationMatte.MatteType,
    for photo: AVCapturePhoto
) -> AVSemanticSegmentationMatte?
```

## Parameters 

`semanticSegmentationMatteType`  

The type of semantic segmentation matte to be replaced or stripped.

`photo`  

The calling instance of AVCapturePhoto.

## Return Value

An instance of AVSemanticSegmentationMatte. To preserve the existing matte, return ```` photo.```AVCapturePhoto/semanticSegmentationMatte(for:)``. To strip the existing one, return  ````nil\`. To replace, provide a replacement AVSemanticSegmentationMatte instance.

## Discussion

This callback is optional. If your delegate doesn’t implement this callback, the existing semantic segmentation matte of the specified type in the in-memory AVCapturePhoto container is written to the file data representation.

## See Also

### Replacing or Removing Metadata

func replacementMetadata(for: AVCapturePhoto) -> [String : Any]?

A callback in which you can provide replacement metadata or direct AVCapturePhoto to strip existing metadata from the flattened file.

func replacementEmbeddedThumbnailPixelBuffer(withPhotoFormat: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>, for: AVCapturePhoto) -> Unmanaged&lt;CVPixelBuffer>?

A callback in which you can provide a replacement embedded thumbnail image with compression settings, or strip the existing embedded thumbnail image from the flattened file.

func replacementDepthData(for: AVCapturePhoto) -> AVDepthData?

A callback in which you can provide replacement depth data or strip existing depth data from the file.

func replacementPortraitEffectsMatte(for: AVCapturePhoto) -> AVPortraitEffectsMatte?

A callback in which you can provide a replacement portrait effects matte, or strip the existing portrait effects matte from the file.

func replacementAppleProRAWCompressionSettings(for: AVCapturePhoto, defaultSettings: [String : Any], maximumBitDepth: Int) -> [String : Any]

Replaces the compression settings the system uses when writing Apple ProRAW data to a Linear DNG file.

