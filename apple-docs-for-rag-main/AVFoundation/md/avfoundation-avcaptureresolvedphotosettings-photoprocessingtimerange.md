

- AVFoundation
- AVCaptureResolvedPhotoSettings
-  photoProcessingTimeRange 

Instance Property

# photoProcessingTimeRange

The time range in which to expect the system to deliver the photo to the delegate.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var photoProcessingTimeRange: CMTimeRange { get }
```

## Discussion

Indicates the processing time range you can expect for this photo to be delivered to your delegate. the .start field of the CMTimeRange is zero-based. In other words, if photoProcessingTimeRange.start is equal to .5 seconds, then the minimum processing time for this photo is .5 seconds. The .start field plus the .duration field of the CMTimeRange indicate the max expected processing time for this photo. Consider implementing a UI affordance if the max processing time is uncomfortably long.

## See Also

### Examining Output Dimensions

var photoDimensions: CMVideoDimensions

The size, in pixels, of the photo image (in a processed format, such as JPEG) that the capture delivers.

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

