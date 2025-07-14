

- AVFoundation
- AVMutableMovie
-  addMutableTracksCopyingSettings(from:options:) 

Instance Method

# addMutableTracksCopyingSettings(from:options:)

Adds one or more empty tracks to the target movie and copies the track settings from the source tracks.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
func addMutableTracksCopyingSettings(
    from existingTracks: [AVAssetTrack],
    options: [String : Any]? = nil
) -> [AVMutableMovieTrack]
```

## Parameters 

`existingTracks`  

An array of asset tracks to be added.

`options`  

A dictionary that contains key for specifying the movie object initialization. Currently, no keys are defined.

## Return Value

An array of AVMutableMovieTrack objects. The index of a track in this array is the same as the index of its source track in the `existingTracks` array.

## Discussion

Properties involving pairs of tracks,such as track references, are copied from the source tracks to the target tracks.

## See Also

### Managing Tracks

func mutableTrack(compatibleWith: AVAssetTrack) -> AVMutableMovieTrack?

Provides a reference to a track from a mutable movie into which you can insert any time range.

func addMutableTrack(withMediaType: AVMediaType, copySettingsFrom: AVAssetTrack?, options: [String : Any]?) -> AVMutableMovieTrack?

Adds an empty track to the target movie.

func removeTrack(AVMovieTrack)

Removes the specified track from the target movie.

