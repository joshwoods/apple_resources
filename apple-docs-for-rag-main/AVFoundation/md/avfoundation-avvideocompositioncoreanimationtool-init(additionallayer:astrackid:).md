

- AVFoundation
- AVVideoCompositionCoreAnimationTool
-  init(additionalLayer:asTrackID:) 

Initializer

# init(additionalLayer:asTrackID:)

Adds a Core Animation layer to the video composition.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
convenience init(
    additionalLayer layer: CALayer,
    asTrackID trackID: CMPersistentTrackID
)
```

## Parameters 

`layer`  

The Core Animation layer to add.

`trackID`  

A track ID to identify the track.

`trackID` should not match any real trackID in the source.

## Return Value

A new Core Animation tool for the layer.

## Discussion

You use this method to include a Core Animation layer as an individual track input in video composition.

Video composition instructions should reference `trackID` where the rendered animation should be included.

## See Also

### Creating a Composition Tool

convenience init(postProcessingAsVideoLayer: CALayer, in: CALayer)

Composes the composited video frame with a Core Animation layer.

convenience init(postProcessingAsVideoLayers: [CALayer], in: CALayer)

Composes the composited video frames with the Core Animation layer.

