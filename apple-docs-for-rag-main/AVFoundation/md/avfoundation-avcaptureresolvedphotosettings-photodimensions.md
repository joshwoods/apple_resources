

- AVFoundation
- AVCaptureResolvedPhotoSettings
-  photoDimensions 

Instance Property

# photoDimensions

The size, in pixels, of the photo image (in a processed format, such as JPEG) that the capture delivers.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
var photoDimensions: CMVideoDimensions { get }
```

## Discussion

The output dimensions of a captured image are set at the moment of capture, depending on device orientation and capture session configuration. (For example, when the capture session includes a video output and video stabilization is in use, captured photos are smaller.)

This property provides the dimensions of the image to be delivered in the photoOutput(_:didFinishProcessingPhoto:error:) method. Use this property in earlier delegate methods to find the size of the image before delivery.

If you do not request capture in a processed format (that is, if you request capture in RAW format only), this property’s value has zero width and zero height.

## See Also

### Examining Output Dimensions

var deferredPhotoProxyDimensions: CMVideoDimensions

The resolved dimensions of the photo proxy when using deferred photo delivery.

var rawPhotoDimensions: CMVideoDimensions

The size, in pixels, of the RAW-format photo image that the capture delivers.

var previewDimensions: CMVideoDimensions

The size, in pixels, of the preview image that the system delivers with the capture.

var embeddedThumbnailDimensions: CMVideoDimensions

The size, in pixels, of the thumbnail image that the capture delivers.

var rawEmbeddedThumbnailDimensions: CMVideoDimensions

The size, in pixels, of the RAW-format embedded thumbnail image that the capture delivers.

var livePhotoMovieDimensions: CMVideoDimensions

The size, in pixels, of the Live Photo movie content that the capture delivers.

var portraitEffectsMatteDimensions: CMVideoDimensions

The size, in pixels, of the portrait effects matte that the capture delivers.

func dimensionsForSemanticSegmentationMatte(ofType: AVSemanticSegmentationMatte.MatteType) -> CMVideoDimensions

Retrieves the resolved dimensions of the semantic segmentation mattes that the photo output delivers.

var photoProcessingTimeRange: CMTimeRange

The time range in which to expect the system to deliver the photo to the delegate.

