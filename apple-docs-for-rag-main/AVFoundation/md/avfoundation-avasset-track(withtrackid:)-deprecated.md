

- AVFoundation
- AVAsset
-  track(withTrackID:) Deprecated

Instance Method

# track(withTrackID:)

Returns a track that contains the specified identifier.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedtvOS 9.0–16.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
func track(withTrackID trackID: CMPersistentTrackID) -> AVAssetTrack?
```

Deprecated

Use loadTrack(withTrackID:completionHandler:) instead.

## Parameters 

`trackID`  

The identifier of the track to retrieve.

## Return Value

An asset track, or `nil` if there is no track with the identifier.

## Discussion

You can call this method without blocking the current thread when the data in the tracks property is already loaded.

