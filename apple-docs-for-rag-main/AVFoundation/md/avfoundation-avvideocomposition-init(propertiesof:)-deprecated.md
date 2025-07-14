

- AVFoundation
- AVVideoComposition
-  init(propertiesOf:) Deprecated

Initializer

# init(propertiesOf:)

Creates a video composition object configured to present the video tracks of the specified asset.

iOS 6.0–18.0DeprecatediPadOS 6.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.9–15.0DeprecatedtvOS 9.0–18.0Deprecated

``` source
init(propertiesOf asset: AVAsset)
```

Deprecated

Use videoCompositionWithPropertiesOfAsset:completionHandler: instead

## Parameters 

`asset`  

The asset whose configuration matches the intended use of the video composition.

## Return Value

A new video composition object.

## Discussion

Apple discourages using this method in iOS 16, tvOS 16, and macOS 13 or later. Create a video composition asynchronously using videoComposition(withPropertiesOf:completionHandler:) instead.

This method creates the video composition object and configures it with the values and instructions suitable for presenting the video tracks of the specified asset. The returned object contains instructions that respect the spatial properties and time ranges of the specified asset’s video tracks. It also configures the object properties in the following way:

- The value of the frameDuration property is short enough to accommodate the greatest nominal frame rate value among the asset’s video tracks, as indicated by the nominalFrameRate property of each track. If all its tracks have a nominal frame rate of `0`, it uses a frame rate of 30 frames per second, with the frame duration set accordingly.

- The value of the renderSize property depends on whether the asset is an AVComposition object. For an AVComposition, the render size is the composition’s naturalSize value, and for other assets, its a size large enough to encompass all of its video tracks.

- The value of the renderScale property is `1.0`.

- The value of the animationTool property is `nil`.

Note

If you specify an asset that doesn’t contain video tracks, this method returns a video composition with no instructions.

## See Also

### Creating a Video Composition

class func videoComposition(withPropertiesOf: AVAsset, completionHandler: (AVVideoComposition?, (any Error)?) -> Void)

Returns a new video composition that’s configured to present the video tracks of the specified asset.

class func videoComposition(with: AVAsset, applyingCIFiltersWithHandler: (AVAsynchronousCIImageFilteringRequest) -> Void, completionHandler: (AVVideoComposition?, (any Error)?) -> Void)

Returns a new video composition that’s configured to apply Core Image filters to each video frame of the specified asset.

class AVAsynchronousCIImageFilteringRequest

An object that supports using Core Image filters to process an individual video frame in a video composition.

init(asset: AVAsset, applyingCIFiltersWithHandler: (AVAsynchronousCIImageFilteringRequest) -> Void)

Creates a video composition configured to apply Core Image filters to each video frame of the specified asset.

Deprecated

