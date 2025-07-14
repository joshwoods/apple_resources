

- AVFoundation
- AVCapturePhotoSettings
-  enabledSemanticSegmentationMatteTypes 

Instance Property

# enabledSemanticSegmentationMatteTypes

An array of semantic segmentation matte types that the photo render pipeline can deliver.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var enabledSemanticSegmentationMatteTypes: [AVSemanticSegmentationMatte.MatteType] { get set }
```

## Discussion

You may set this property to the array of matte types you’d like delivered with AVCapturePhoto. The array may only contain values present in availableSemanticSegmentationMatteTypes.

The default value of this property is an empty array.

## See Also

### Capturing Semantic Segmentation Mattes

var embedsSemanticSegmentationMattesInPhoto: Bool

A Boolean value that specifies whether to write the enabled semantic segmentation matte types captured with this photo to the photo’s file structure.

