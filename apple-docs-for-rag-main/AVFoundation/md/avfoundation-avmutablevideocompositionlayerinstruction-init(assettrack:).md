

- AVFoundation
- AVMutableVideoCompositionLayerInstruction
-  init(assetTrack:) 

Initializer

# init(assetTrack:)

Creates a new mutable video composition layer instruction for the given track.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
convenience init(assetTrack track: AVAssetTrack)
```

## Parameters 

`track`  

The asset track to which to apply the instruction.

## Return Value

A new mutable video composition layer instruction with no transform or opacity ramps and trackID initialized to the track ID of `track`.

