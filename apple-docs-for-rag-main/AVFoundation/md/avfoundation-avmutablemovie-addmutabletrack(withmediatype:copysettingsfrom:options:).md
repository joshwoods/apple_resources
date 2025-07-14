

- AVFoundation
- AVMutableMovie
-  addMutableTrack(withMediaType:copySettingsFrom:options:) 

Instance Method

# addMutableTrack(withMediaType:copySettingsFrom:options:)

Adds an empty track to the target movie.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
func addMutableTrack(
    withMediaType mediaType: AVMediaType,
    copySettingsFrom track: AVAssetTrack?,
    options: [String : Any]? = nil
) -> AVMutableMovieTrack?
```

## Parameters 

`mediaType`  

The media type for the new track.

`track`  

An AVAssetTrack containing the desired track settings to be transferred. Set to `nil` to create a track with default settings.

`options`  

A dictionary that contains key for specifying the movie object initialization. Currently, no keys are defined.

## Return Value

An AVMutableMovieTrack object.

## See Also

### Managing Tracks

func mutableTrack(compatibleWith: AVAssetTrack) -> AVMutableMovieTrack?

Provides a reference to a track from a mutable movie into which you can insert any time range.

func addMutableTracksCopyingSettings(from: [AVAssetTrack], options: [String : Any]?) -> [AVMutableMovieTrack]

Adds one or more empty tracks to the target movie and copies the track settings from the source tracks.

func removeTrack(AVMovieTrack)

Removes the specified track from the target movie.

