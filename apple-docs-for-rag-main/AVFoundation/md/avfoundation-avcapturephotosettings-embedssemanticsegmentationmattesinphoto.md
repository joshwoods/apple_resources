

- AVFoundation
- AVCapturePhotoSettings
-  embedsSemanticSegmentationMattesInPhoto 

Instance Property

# embedsSemanticSegmentationMattesInPhoto

A Boolean value that specifies whether to write the enabled semantic segmentation matte types captured with this photo to the photo’s file structure.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var embedsSemanticSegmentationMattesInPhoto: Bool { get set }
```

## Discussion

Semantic segmentation mattes are only supported in HEIF and JPEG. The photo output ignores this property if you set enabledSemanticSegmentationMatteTypes to an empty array.

The property’s default value is true.

Important

Enabling semantic segmentation matte delivery requires a lengthy reconfiguration of the capture render pipeline. If you intend to capture semantic segmentation mattes, set this property to true before calling the capture session’s startRunning() method.

## See Also

### Capturing Semantic Segmentation Mattes

var enabledSemanticSegmentationMatteTypes: [AVSemanticSegmentationMatte.MatteType]

An array of semantic segmentation matte types that the photo render pipeline can deliver.

