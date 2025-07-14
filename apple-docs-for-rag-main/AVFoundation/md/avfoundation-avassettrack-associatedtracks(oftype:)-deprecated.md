

- AVFoundation
- AVAssetTrack
-  associatedTracks(ofType:) Deprecated

Instance Method

# associatedTracks(ofType:)

Returns an array of associated tracks that have the specified association type.

iOS 7.0–16.0DeprecatediPadOS 7.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.9–13.0DeprecatedtvOS 9.0–16.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
func associatedTracks(ofType trackAssociationType: AVAssetTrack.AssociationType) -> [AVAssetTrack]
```

Deprecated

Use loadAssociatedTracks(ofType:completionHandler:) instead.

## Parameters 

`trackAssociationType`  

The requested track association type.

## Return Value

An array of tracks matching the specified track association type, or an empty array if none are found.

## Discussion

Apple discourages using this method in iOS 15, tvOS 15, macOS 12, and watchOS 8 or later. Load associated tracks asynchronously using loadAssociatedTracks(ofType:completionHandler:) instead.

You can call this method without blocking the current thread after you’ve loaded the availableTrackAssociationTypes property.

