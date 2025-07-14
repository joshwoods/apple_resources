

- AVFoundation
- AVCapturePhotoOutput
-  enabledSemanticSegmentationMatteTypes 

Instance Property

# enabledSemanticSegmentationMatteTypes

The semantic segmentation matte types that the photo render pipeline delivers.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var enabledSemanticSegmentationMatteTypes: [AVSemanticSegmentationMatte.MatteType] { get set }
```

## Discussion

Set this property value to the array of matte types you’d like delivered with your primary photos. The array may only contain values present in availableSemanticSegmentationMatteTypes.

The default value of this property is an empty array.

Important

Enabling semantic segmentation matte delivery requires a lengthy reconfiguration of the capture render pipeline. If you intend to capture semantic segmentation mattes, set this property to your desired types before calling the capture session’s startRunning() method.

## See Also

### Getting Segmentation Mattes

var availableSemanticSegmentationMatteTypes: [AVSemanticSegmentationMatte.MatteType]

An array of semantic segmentation matte types that may be captured and delivered along with the primary photo.

