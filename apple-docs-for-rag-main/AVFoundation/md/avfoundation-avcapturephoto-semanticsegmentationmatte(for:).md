

- AVFoundation
- AVCapturePhoto
-  semanticSegmentationMatte(for:) 

Instance Method

# semanticSegmentationMatte(for:)

Retrieves the semantic segmentation matte associated with this photo.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
func semanticSegmentationMatte(for semanticSegmentationMatteType: AVSemanticSegmentationMatte.MatteType) -> AVSemanticSegmentationMatte?
```

## Parameters 

`semanticSegmentationMatteType`  

The type of semantic segmentation matte to retrieve from the photo.

## Return Value

An instance of AVSemanticSegmentationMatte, or `nil` of you didn’t request semantic segmentation matte delivery or if no mattes of the specified type were found.

## Discussion

If you requested one or more semantic segmentation mattes by calling enabledSemanticSegmentationMatteTypes with a nonempty array of types, this property offers access to the resulting AVSemanticSegmentationMatte objects.

Note

Semantic segmentation mattes are only embedded in the photo’s internal file format container if you set embedsSemanticSegmentationMattesInPhoto to true.

