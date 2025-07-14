

- AVFoundation
- Photo capture
- Capturing Still and Live Photos
-  Capturing Thumbnail and Preview Images 

Article

# Capturing Thumbnail and Preview Images

Enable delivery of reduced-size images with the main image in a photo capture.

## Overview

Generating your own preview or thumbnail images from high-resolution source images can be difficult and time-consuming. Instead, use AVCapturePhotoOutput to get easy, fast preview and thumbnail generation as part of your capture process.

In the capture system, the names *preview* and *thumbnail* have specific meanings:

- A *preview image* is a reduced-size (screen resolution or smaller) version of the photo, in an uncompressed format, delivered only in memory for purposes of displaying feedback shortly after capture. For example, the system Camera app displays a preview image of the last captured photo.

- A *thumbnail image* is a smaller version of the photo, encoded in a compressed format and embedded in the output image file for use by other software. For example, image browsers reading a folder full of images can preview the contents of many files without reading and decoding each file’s entire contents.

You can add preview images, thumbnail images, or both with minor additions to any AVCapturePhotoOutput workflow (see Capturing Still and Live Photos and related topics).

### Choose Settings

After you create an AVCapturePhotoSettings object for the kind of photo you plan to shoot, use its previewPhotoFormat dictionary to specify the format and size of preview image you want.

```
if photoSettings.availablePreviewPhotoPixelFormatTypes.count > 0 {
    photoSettings.previewPhotoFormat = [
        kCVPixelBufferPixelFormatTypeKey : photoSettings.availablePreviewPhotoPixelFormatTypes.first!,
        kCVPixelBufferWidthKey : 512,
        kCVPixelBufferHeightKey : 512
    ] as [String: Any]
}

```

To request that a thumbnail version of the photo be embedded in the resulting image file, use the photo settings object’s embeddedThumbnailPhotoFormat dictionary to specify the format and size of the thumbnail.

```
photoSettings.embeddedThumbnailPhotoFormat = [
    AVVideoCodecKey: AVVideoCodecType.jpeg,
    AVVideoWidthKey: 1024,
    AVVideoHeightKey: 1024,
]
```

### Handle Results

When the photo output calls your delegate’s photoOutput(_:didFinishProcessingPhoto:error:) method, you can get the preview image from the AVCapturePhoto previewPixelBuffer property. A pixel buffer provides direct access to pixel data, so you can process or display it using other graphics technologies such as Metal, Vision, or Core Image. One way to simply display the preview image in your UI is to use Core Image to wrap the buffer in a UIImage object:

```
func showPreview(for photo: AVCapturePhoto) {
    guard let previewPixelBuffer = photo.previewPixelBuffer else { return }
    let ciImage = CIImage(cvPixelBuffer: previewPixelBuffer)
    let uiImage = UIImage(ciImage: ciImage)
    self.imageView.image = uiImage
}

```

If you requested an embedded thumbnail image, that image isn’t directly accessible from the AVCapturePhoto object—it’s embedded in the image file data that you get by calling the photo object’s fileDataRepresentation() method.

## See Also

### More Capture Options

Capturing Photos with Depth

Get a depth map with a photo to create effects like the system camera’s Portrait mode (on compatible devices).

Capturing a Bracketed Photo Sequence

Capture several photos at once, varying parameters like exposure duration or light sensitivity.

Capturing Uncompressed Image Data

Get processed image data without compression to use for filtering or lossless output.

