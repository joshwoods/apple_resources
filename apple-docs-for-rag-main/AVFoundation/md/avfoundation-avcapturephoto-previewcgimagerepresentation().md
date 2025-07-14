

- AVFoundation
- AVCapturePhoto
-  previewCGImageRepresentation() 

Instance Method

# previewCGImageRepresentation()

Extracts and returns the captured photo’s preview image as a Core Graphics image object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
func previewCGImageRepresentation() -> CGImage?
```

## Return Value

A Core Graphics image representation of the captured photo, or `nil` if either the image cannot be converted or a preview image was not requested as part of the photo capture.

## See Also

### Packaging Data for File Output

func fileDataRepresentation(with: any AVCapturePhotoFileDataRepresentationCustomizer) -> Data?

Gets a customized representation of the photo data.

protocol AVCapturePhotoFileDataRepresentationCustomizer

A protocol that defines the methods to implement to customize the packaging of photo data.

func fileDataRepresentation() -> Data?

Generates and returns a flat data representation of the photo and its attachments.

func cgImageRepresentation() -> CGImage?

Extracts and returns the captured photo’s primary image as a Core Graphics image object.

func fileDataRepresentation(withReplacementMetadata: [String : Any]?, replacementEmbeddedThumbnailPhotoFormat: [String : Any]?, replacementEmbeddedThumbnailPixelBuffer: CVPixelBuffer?, replacementDepthData: AVDepthData?) -> Data?

Generates and returns a flat data representation of the photo using the specified replacements for some or all of its attachments.

Deprecated

