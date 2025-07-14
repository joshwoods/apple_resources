

- AVFoundation
- AVCapturePhoto
-  fileDataRepresentation() 

Instance Method

# fileDataRepresentation()

Generates and returns a flat data representation of the photo and its attachments.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
func fileDataRepresentation() -> Data?
```

## Return Value

Data appropriate for writing to a file of the type specified when requesting photo capture, or `nil` if the photo and attachment data cannot be flattened.

## Mentioned in 

Saving Captured Photos

Capturing Thumbnail and Preview Images

Configuring Camera Capture to Collect a Portrait Effects Matte

Capturing Uncompressed Image Data

Capturing Photos with Depth

## Discussion

When you request a photo capture with the AVCapturePhotoOutput capturePhoto(with:delegate:) method, the AVCapturePhotoSettings object you provide specifies image data formats (such as JPEG and HEVC) and container file formats (such as JFIF and HEIF) for the resulting image file. Calling this method formats and packages the image pixel buffer, along with metadata and other attachments created during capture (such as preview photos and depth maps), into data appropriate for writing to a file of that type.

## See Also

### Packaging Data for File Output

func fileDataRepresentation(with: any AVCapturePhotoFileDataRepresentationCustomizer) -> Data?

Gets a customized representation of the photo data.

protocol AVCapturePhotoFileDataRepresentationCustomizer

A protocol that defines the methods to implement to customize the packaging of photo data.

func cgImageRepresentation() -> CGImage?

Extracts and returns the captured photo’s primary image as a Core Graphics image object.

func previewCGImageRepresentation() -> CGImage?

Extracts and returns the captured photo’s preview image as a Core Graphics image object.

func fileDataRepresentation(withReplacementMetadata: [String : Any]?, replacementEmbeddedThumbnailPhotoFormat: [String : Any]?, replacementEmbeddedThumbnailPixelBuffer: CVPixelBuffer?, replacementDepthData: AVDepthData?) -> Data?

Generates and returns a flat data representation of the photo using the specified replacements for some or all of its attachments.

Deprecated

