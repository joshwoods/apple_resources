

- AVFoundation
- AVURLAsset
-  compatibleTrack(for:) Deprecated

Instance Method

# compatibleTrack(for:)

Returns an asset track from which you can insert any time range into a given composition track.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedtvOS 9.0–16.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
func compatibleTrack(for compositionTrack: AVCompositionTrack) -> AVAssetTrack?
```

Deprecated

Use findCompatibleTrack(for:completionHandler:) instead.

## Parameters 

`compositionTrack`  

The composition track.

## Return Value

An asset track managed by the asset from which any time range can be inserted into a given composition track.

## Discussion

Apple discourages using this method in iOS 15, tvOS 15, macOS 12, and watchOS 8 or later. Load compatible tracks asynchronously using findCompatibleTrack(for:completionHandler:) instead.

This method is the logical complement of mutableTrack(compatibleWith:).

