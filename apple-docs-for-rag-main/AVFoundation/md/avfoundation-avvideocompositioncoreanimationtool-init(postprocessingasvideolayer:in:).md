

- AVFoundation
- AVVideoCompositionCoreAnimationTool
-  init(postProcessingAsVideoLayer:in:) 

Initializer

# init(postProcessingAsVideoLayer:in:)

Composes the composited video frame with a Core Animation layer.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
convenience init(
    postProcessingAsVideoLayer videoLayer: CALayer,
    in animationLayer: CALayer
)
```

## Parameters 

`videoLayer`  

A video layer.

`animationLayer`  

An animation layer.

## Return Value

A new animation tool for the composition.

## Discussion

Place composited video frames in `videoLayer` and render `animationLayer` to produce the final frame.

The `videoLayer` should be in the `animationLayer` sublayer tree. The `animationLayer` should not come from, or be added to, another layer tree.

## See Also

### Creating a Composition Tool

convenience init(additionalLayer: CALayer, asTrackID: CMPersistentTrackID)

Adds a Core Animation layer to the video composition.

convenience init(postProcessingAsVideoLayers: [CALayer], in: CALayer)

Composes the composited video frames with the Core Animation layer.

