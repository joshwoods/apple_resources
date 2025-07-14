

- AVFoundation
- AVVideoCompositionCoreAnimationTool
-  init(postProcessingAsVideoLayers:in:) 

Initializer

# init(postProcessingAsVideoLayers:in:)

Composes the composited video frames with the Core Animation layer.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
convenience init(
    postProcessingAsVideoLayers videoLayers: [CALayer],
    in animationLayer: CALayer
)
```

## Parameters 

`videoLayers`  

An array containing the video layers

`animationLayer`  

The animation layer.

## Return Value

A new `AVVideoCompositionCoreAnimationTool` instance with the composited video frames and the rendered animation layer.

## Discussion

Duplicates the composited video frames in each videoLayer and renders animationLayer to produce the final frame. The `videoLayers` should be in `animationLayer`’s sublayer tree.

The `animationLayer` should not come from, or be added to, another layer tree.

Note

On iOS, a layer instance backing a UIView usually have their content flipped, as defined by the contentsAreFlipped() method. It may be required to insert a CALayer instance with its isGeometryFlipped property set to true in the layer hierarchy to get the same result when attaching a layer to the receiver when the layer backs a UIView.

## See Also

### Creating a Composition Tool

convenience init(additionalLayer: CALayer, asTrackID: CMPersistentTrackID)

Adds a Core Animation layer to the video composition.

convenience init(postProcessingAsVideoLayer: CALayer, in: CALayer)

Composes the composited video frame with a Core Animation layer.

