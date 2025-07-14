

- AVFoundation
-  AVCapturePhotoFileDataRepresentationCustomizer 

Protocol

# AVCapturePhotoFileDataRepresentationCustomizer

A protocol that defines the methods to implement to customize the packaging of photo data.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
protocol AVCapturePhotoFileDataRepresentationCustomizer : NSObjectProtocol
```

## Mentioned in 

Capturing Photos in RAW and Apple ProRAW Formats

## Overview

AVCapturePhoto is a wrapper representing a photo in a file container. To flatten the photo to an NSData object to write to file, call fileDataRepresentation(). For more complex flattening operations such as replacing or stripping metadata, call fileDataRepresentation(with:) and provide a delegate for customized replacement or stripping behavior. This delegate’s methods are called synchronously before the flattening process begins.

## Topics

### Replacing or Removing Metadata

func replacementMetadata(for: AVCapturePhoto) -> [String : Any]?

A callback in which you can provide replacement metadata or direct AVCapturePhoto to strip existing metadata from the flattened file.

func replacementEmbeddedThumbnailPixelBuffer(withPhotoFormat: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>, for: AVCapturePhoto) -> Unmanaged&lt;CVPixelBuffer>?

A callback in which you can provide a replacement embedded thumbnail image with compression settings, or strip the existing embedded thumbnail image from the flattened file.

func replacementDepthData(for: AVCapturePhoto) -> AVDepthData?

A callback in which you can provide replacement depth data or strip existing depth data from the file.

func replacementPortraitEffectsMatte(for: AVCapturePhoto) -> AVPortraitEffectsMatte?

A callback in which you can provide a replacement portrait effects matte, or strip the existing portrait effects matte from the file.

func replacementSemanticSegmentationMatte(ofType: AVSemanticSegmentationMatte.MatteType, for: AVCapturePhoto) -> AVSemanticSegmentationMatte?

Replaces or removes the semantic segmentation matte of the specified type from the flattened file data representation.

func replacementAppleProRAWCompressionSettings(for: AVCapturePhoto, defaultSettings: [String : Any], maximumBitDepth: Int) -> [String : Any]

Replaces the compression settings the system uses when writing Apple ProRAW data to a Linear DNG file.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Packaging Data for File Output

func fileDataRepresentation(with: any AVCapturePhotoFileDataRepresentationCustomizer) -> Data?

Gets a customized representation of the photo data.

func fileDataRepresentation() -> Data?

Generates and returns a flat data representation of the photo and its attachments.

func cgImageRepresentation() -> CGImage?

Extracts and returns the captured photo’s primary image as a Core Graphics image object.

func previewCGImageRepresentation() -> CGImage?

Extracts and returns the captured photo’s preview image as a Core Graphics image object.

func fileDataRepresentation(withReplacementMetadata: [String : Any]?, replacementEmbeddedThumbnailPhotoFormat: [String : Any]?, replacementEmbeddedThumbnailPixelBuffer: CVPixelBuffer?, replacementDepthData: AVDepthData?) -> Data?

Generates and returns a flat data representation of the photo using the specified replacements for some or all of its attachments.

Deprecated

