

- AVFoundation
- AVCapturePhotoOutput
-  availableSemanticSegmentationMatteTypes 

Instance Property

# availableSemanticSegmentationMatteTypes

An array of semantic segmentation matte types that may be captured and delivered along with the primary photo.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var availableSemanticSegmentationMatteTypes: [AVSemanticSegmentationMatte.MatteType] { get }
```

## Discussion

This property returns the array of semantic segmentation types that’s available given the current session configuration.

This property is key-value observable.

Important

The value of this property may change when switching cameras or formats. When this property changes, enabledSemanticSegmentationMatteTypes reverts to an empty array. If you’ve previously opted in for delivery of one or more semantic segmentation mattes, you need to set up your enabledSemanticSegmentationMatteTypes again.

## See Also

### Getting Segmentation Mattes

var enabledSemanticSegmentationMatteTypes: [AVSemanticSegmentationMatte.MatteType]

The semantic segmentation matte types that the photo render pipeline delivers.

