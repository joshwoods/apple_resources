

- AVFoundation
- AVAsset
-  tracks(withMediaType:) Deprecated

Instance Method

# tracks(withMediaType:)

Returns tracks that contain media of a specified type.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedtvOS 9.0–16.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
func tracks(withMediaType mediaType: AVMediaType) -> [AVAssetTrack]
```

Deprecated

Use loadTracks(withMediaType:completionHandler:)

## Parameters 

`mediaType`  

The media type of the tracks to return.

## Return Value

An array of tracks, which is empty if there are no tracks with the media type.

## Discussion

\You can call this method without blocking the current thread when the data in the tracks property is already loaded.

