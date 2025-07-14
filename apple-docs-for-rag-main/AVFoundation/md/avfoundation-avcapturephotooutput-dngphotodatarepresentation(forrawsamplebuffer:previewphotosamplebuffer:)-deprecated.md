

- AVFoundation
- AVCapturePhotoOutput
-  dngPhotoDataRepresentation(forRawSampleBuffer:previewPhotoSampleBuffer:) Deprecated

Type Method

# dngPhotoDataRepresentation(forRawSampleBuffer:previewPhotoSampleBuffer:)

Returns data in digital negative (DNG) format corresponding to the captured RAW photo in the specified sample buffer.

iOS 10.0–11.0DeprecatediPadOS 10.0–11.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
class func dngPhotoDataRepresentation(
    forRawSampleBuffer rawSampleBuffer: CMSampleBuffer,
    previewPhotoSampleBuffer: CMSampleBuffer?
) -> Data?
```

Deprecated

In iOS 11 and later, implement the photoOutput(_:didFinishProcessingPhoto:error:) method in your capture delegate and use the fileDataRepresentation() method of the resulting AVCapturePhoto object.

## Parameters 

`rawSampleBuffer`  

A sample buffer containing the RAW photo capture result to be formatted for output.

`previewPhotoSampleBuffer`  

An optional additional sample buffer containing a preview-resolution version of the photo capture result, to be added to the DNG output as a thumbnail image. Pass `nil` to skip adding a preview image to the output.

## Return Value

A data object containing a DNG representation of the requested photo capture results, or `nil` if the sample buffers cannot be packaged for output.

## Discussion

After you request a photo capture with the capturePhoto(with:delegate:) method, the photo capture output delivers results to your delegate as one or more CMSampleBuffer objects. (See the photoOutput(_:didFinishProcessingRawPhoto:previewPhoto:resolvedSettings:bracketSettings:error:) method.) To repackage the sample buffer’s content for output as a DNG file, use this class method. Optionally, you can include metadata in the resulting DNG output by attaching it to the sample buffer before calling this method.

Important

The `rawSampleBuffer` parameter must reference a sample buffer from a RAW capture. See the rawPhotoPixelFormatType property for photo capture settings.

## See Also

### Getting Formatted Output

class func jpegPhotoDataRepresentation(forJPEGSampleBuffer: CMSampleBuffer, previewPhotoSampleBuffer: CMSampleBuffer?) -> Data?

Returns data in JPEG format corresponding to the captured photo in the specified sample buffer.

Deprecated

