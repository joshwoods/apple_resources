

- AVFoundation
- AVCaptureResolvedPhotoSettings
-  dimensionsForSemanticSegmentationMatte(ofType:) 

Instance Method

# dimensionsForSemanticSegmentationMatte(ofType:)

Retrieves the resolved dimensions of the semantic segmentation mattes that the photo output delivers.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
func dimensionsForSemanticSegmentationMatte(ofType semanticSegmentationMatteType: AVSemanticSegmentationMatte.MatteType) -> CMVideoDimensions
```

## Parameters 

`semanticSegmentationMatteType`  

The segmentation matte type for which to retrieve dimensions.

## Return Value

A CMVideoDimensions structure that provides the height and width of the image mattes.

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

var photoProcessingTimeRange: CMTimeRange

The time range in which to expect the system to deliver the photo to the delegate.

