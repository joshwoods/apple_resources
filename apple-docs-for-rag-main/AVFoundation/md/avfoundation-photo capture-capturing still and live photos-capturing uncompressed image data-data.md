

- AVFoundation
- Photo capture
- Capturing Still and Live Photos
-  Capturing Uncompressed Image Data 

Article

# Capturing Uncompressed Image Data

Get processed image data without compression to use for filtering or lossless output.

## Overview

Typical photography workflows save images in a compressed format such as HEIF/HEVC or JPEG. These formats use lossy compression to strike a balance between preserving noticeable details in the image and reducing its data storage requirements. However, sometimes it’s more helpful to work with uncompressed image data—for example, some image processing and analysis algorithms can be confused by the visual artifacts introduced by lossy compression.

Note

Uncompressed image data is not to be confused with unprocessed, or RAW, image data. RAW data is minimally altered data direct from a camera’s image sensor. Uncompressed image data has been processed to create a displayable image, but hasn’t been compressed to create a small file.

In iOS, capturing uncompressed image data requires minor changes to the basic photography workflow covered in Capturing Still and Live Photos.

### Choose Uncompressed Format Settings

To capture in an uncompressed format, create a photo settings object with init(format:). In the format dictionary, specify the kCVPixelBufferPixelFormatTypeKey with one of the values listed in the photo output’s availablePhotoPixelFormatTypes array. The example below chooses a 32-bit BGRA pixel format, which is useful in some GPU processing workflows:

```
// Choose a 32-bit BGRA pixel format and verify the camera supports it.
let pixelFormatType = kCVPixelFormatType_32BGRA
guard self.photoOutput.availablePhotoPixelFormatTypes.contains(pixelFormatType) else { return }
let photoSettings = AVCapturePhotoSettings(format:
    [ kCVPixelBufferPixelFormatTypeKey as String : pixelFormatType ])

// Shoot the photo, using a custom class to handle capture delegate callbacks.
let layerOrientation = previewView.videoPreviewLayer.connection!.videoOrientation
let colorSpace = self.videoCaptureDevice.activeColorSpace
let captureProcessor = UncompressedCaptureProcessor(orientation: layerOrientation,
                                                    colorSpace: colorSpace)
self.photoOutput.capturePhoto(with: photoSettings, delegate: captureProcessor)

```

### Handle Results

As with other formats, you receive uncompressed data capture results to your delegate’s photoOutput(_:didFinishProcessingPhoto:error:) method as an AVCapturePhoto object. To access the uncompressed pixel data directly, use the photo’s pixelBuffer property.

For example, the following code applies a Core Image filter directly to the pixel buffer and writes the filtered image to a PNG file:

```
class UncompressedCaptureProcessor: NSObject, AVCapturePhotoCaptureDelegate {

    // Hold on to the separately delivered RAW and compressed photo data until capture is finished.
    func photoOutput(_ output: AVCapturePhotoOutput, didFinishProcessingPhoto photo: AVCapturePhoto, error: Error?) {
        guard error != nil else { print("Error capturing photo: \(error!)"); return }

        // Create a CIImage from the pixel buffer and apply a filter
        let image = CIImage(cvPixelBuffer: photo.pixelBuffer!)
        let imageOrientation = self.imageOrientation(for: videoOrientation)
        let filteredImage = image.oriented(imageOrientation)
            .applyingFilter("CIPhotoEffectNoir", parameters: [:])

        let imageColorSpace = self.imageColorSpace(for: colorSpace)
        guard let pngData = CIContext()
            .pngRepresentation(of: filteredImage, format: kCIFormatBGRA8, colorSpace: imageColorSpace)
            else { print("Error creating filtered PNG image"); return }
        self.exportToFile(pngData)
    }
}
```

Alternatively, to get an uncompressed photo ready for writing to a file, use the photo’s fileDataRepresentation() method to get the data formatted as a TIFF file.

## See Also

### More Capture Options

Capturing Photos with Depth

Get a depth map with a photo to create effects like the system camera’s Portrait mode (on compatible devices).

Capturing a Bracketed Photo Sequence

Capture several photos at once, varying parameters like exposure duration or light sensitivity.

Capturing Thumbnail and Preview Images

Enable delivery of reduced-size images with the main image in a photo capture.

