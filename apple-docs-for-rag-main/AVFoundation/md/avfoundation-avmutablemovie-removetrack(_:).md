

- AVFoundation
- AVMutableMovie
-  removeTrack(\_:) 

Instance Method

# removeTrack(\_:)

Removes the specified track from the target movie.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
func removeTrack(_ track: AVMovieTrack)
```

## Parameters 

`track`  

The movie to be removed.

## See Also

### Managing Tracks

func mutableTrack(compatibleWith: AVAssetTrack) -> AVMutableMovieTrack?

Provides a reference to a track from a mutable movie into which you can insert any time range.

func addMutableTrack(withMediaType: AVMediaType, copySettingsFrom: AVAssetTrack?, options: [String : Any]?) -> AVMutableMovieTrack?

Adds an empty track to the target movie.

func addMutableTracksCopyingSettings(from: [AVAssetTrack], options: [String : Any]?) -> [AVMutableMovieTrack]

Adds one or more empty tracks to the target movie and copies the track settings from the source tracks.

