

- AVFoundation
- AVMutableAudioMixInputParameters
-  init(track:) 

Initializer

# init(track:)

Creates a mutable input parameters object for a given track.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
convenience init(track: AVAssetTrack?)
```

## Parameters 

`track`  

The track to associate with the input parameters object.

## Return Value

A mutable input parameters object with no volume ramps and trackID set to `track`’s identifier.

