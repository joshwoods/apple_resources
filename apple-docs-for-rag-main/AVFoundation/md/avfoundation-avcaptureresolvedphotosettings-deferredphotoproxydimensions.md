

- AVFoundation
- AVCaptureResolvedPhotoSettings
-  deferredPhotoProxyDimensions 

Instance Property

# deferredPhotoProxyDimensions

The resolved dimensions of the photo proxy when using deferred photo delivery.

iOS 17.0+iPadOS 17.0+

``` source
var deferredPhotoProxyDimensions: CMVideoDimensions { get }
```

## Discussion

When the system returns an AVCaptureDeferredPhotoProxy, the photoDimensions property of this object represents the dimensions of the final photo. If you don’t opt in to deferred photo delivery, this value has a width and height of 0.

## See Also

### Examining Output Dimensions

var photoDimensions: CMVideoDimensions

The size, in pixels, of the photo image (in a processed format, such as JPEG) that the capture delivers.

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

