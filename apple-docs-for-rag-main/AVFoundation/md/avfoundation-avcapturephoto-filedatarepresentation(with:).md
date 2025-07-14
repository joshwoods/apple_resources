

- AVFoundation
- AVCapturePhoto
-  fileDataRepresentation(with:) 

Instance Method

# fileDataRepresentation(with:)

Gets a customized representation of the photo data.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
func fileDataRepresentation(with customizer: any AVCapturePhotoFileDataRepresentationCustomizer) -> Data?
```

## Parameters 

`customizer`  

An object that customizes the returned metadata, image thumbnail, or depth data.

## Return Value

A data representation of the photo.

## Mentioned in 

Capturing Photos in RAW and Apple ProRAW Formats

Configuring Camera Capture to Collect a Portrait Effects Matte

## See Also

### Packaging Data for File Output

protocol AVCapturePhotoFileDataRepresentationCustomizer

A protocol that defines the methods to implement to customize the packaging of photo data.

func fileDataRepresentation() -> Data?

Generates and returns a flat data representation of the photo and its attachments.

func cgImageRepresentation() -> CGImage?

Extracts and returns the captured photo’s primary image as a Core Graphics image object.

func previewCGImageRepresentation() -> CGImage?

Extracts and returns the captured photo’s preview image as a Core Graphics image object.

func fileDataRepresentation(withReplacementMetadata: [String : Any]?, replacementEmbeddedThumbnailPhotoFormat: [String : Any]?, replacementEmbeddedThumbnailPixelBuffer: CVPixelBuffer?, replacementDepthData: AVDepthData?) -> Data?

Generates and returns a flat data representation of the photo using the specified replacements for some or all of its attachments.

Deprecated

