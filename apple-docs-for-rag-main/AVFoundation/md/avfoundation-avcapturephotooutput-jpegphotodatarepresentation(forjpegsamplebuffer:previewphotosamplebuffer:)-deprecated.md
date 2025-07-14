

- AVFoundation
- AVCapturePhotoOutput
-  jpegPhotoDataRepresentation(forJPEGSampleBuffer:previewPhotoSampleBuffer:) Deprecated

Type Method

# jpegPhotoDataRepresentation(forJPEGSampleBuffer:previewPhotoSampleBuffer:)

Returns data in JPEG format corresponding to the captured photo in the specified sample buffer.

iOS 10.0–11.0DeprecatediPadOS 10.0–11.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
class func jpegPhotoDataRepresentation(
    forJPEGSampleBuffer JPEGSampleBuffer: CMSampleBuffer,
    previewPhotoSampleBuffer: CMSampleBuffer?
) -> Data?
```

Deprecated

In iOS 11 and later, implement the photoOutput(_:didFinishProcessingPhoto:error:) method in your capture delegate and use the fileDataRepresentation() method of the resulting AVCapturePhoto object.

## Parameters 

`JPEGSampleBuffer`  

A sample buffer containing the JPEG photo capture result to be formatted for output.

`previewPhotoSampleBuffer`  

An optional additional sample buffer containing a preview-resolution version of the photo capture result, to be added to the JPEG output as a thumbnail image. Pass `nil` to skip adding a preview image to the output.

## Return Value

A data object containing a JPEG representation of the requested photo capture results, or `nil` if the sample buffers cannot be packaged for output.

## Discussion

After you request a photo capture with the capturePhoto(with:delegate:) method, the photo capture output delivers results to your delegate as one or more CMSampleBuffer objects. (See the photoOutput(_:didFinishProcessingPhoto:previewPhoto:resolvedSettings:bracketSettings:error:) method.) To repackage the sample buffer’s content for output as a JPEG file, use this class method. Optionally, you can include metadata in the resulting JPEG output by attaching it to the sample buffer before calling this method.

Important

The `jpegSampleBuffer` parameter must reference a sample buffer from a JPEG capture. See the format property for photo capture settings.

## See Also

### Getting Formatted Output

class func dngPhotoDataRepresentation(forRawSampleBuffer: CMSampleBuffer, previewPhotoSampleBuffer: CMSampleBuffer?) -> Data?

Returns data in digital negative (DNG) format corresponding to the captured RAW photo in the specified sample buffer.

Deprecated

