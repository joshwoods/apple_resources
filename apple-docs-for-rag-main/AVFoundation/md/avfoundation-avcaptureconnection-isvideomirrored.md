

- AVFoundation
- AVCaptureConnection
-  isVideoMirrored 

Instance Property

# isVideoMirrored

A Boolean value that indicates whether the connection horizontally flips the video flowing through it.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
var isVideoMirrored: Bool { get set }
```

## Discussion

You can apply a mirror-image effect to a video flowing through the connection by setting the value to true. The mirroring effect only applies to video or depth connections, similar to videoRotationAngle, and if isVideoMirroringSupported is true.

Not all capture connections mirror each frame. For example, a video connection to an AVCaptureMovieFileOutput or AVCapturePhotoOutput instance applies the mirror effect with a QuickTime track matrix or with EXIF tags, respectively.

Capture connections to AVCaptureVideoDataOutput and AVCaptureDepthDataOutput instances mirror video frames they provide to their captureOutput(_:didOutput:from:) and depthDataOutput(_:didOutput:timestamp:connection:) delegate methods, respectively. Each AVCaptureVideoDataOutput instance uses hardware acceleration to mirror every frame.

Tip

Avoid potential performance issues by only mirroring video with a capture connection when necessary.

You can mirror the video of a movie file you record with an AVAssetWriter instance by applying a scale factor to the transform property of its AVAssetWriterInput. For example, you can horizontally flip an image by scaling the x-axis by `-1`. This approach avoids the performance costs that come with rotating each video frame.

```
func horizontallyFlipInput(_ assetInput: AVAssetWriterInput) {
    let horiztonalFlip = CGAffineTransform(scaleX: -1.0, y: 1.0)

    assetInput.transform = assetInput.transform.concatenating(horiztonalFlip)
}
```

## See Also

### Mirroring a video

var isVideoMirroringSupported: Bool

A Boolean value that indicates whether the connection supports video mirroring.

var automaticallyAdjustsVideoMirroring: Bool

A Boolean value that indicates whether you can enable mirroring based on a session’s configuration.

