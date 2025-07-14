

- AVFoundation
- AVAsset
-  tracks(withMediaCharacteristic:) Deprecated

Instance Method

# tracks(withMediaCharacteristic:)

Returns an array of asset tracks matching the specified media characteristic.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedtvOS 9.0–16.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
func tracks(withMediaCharacteristic mediaCharacteristic: AVMediaCharacteristic) -> [AVAssetTrack]
```

Deprecated

Use loadTracks(withMediaCharacteristic:completionHandler:) instead

## Parameters 

`mediaCharacteristic`  

The media characteristic of the tracks to return.

## Return Value

An array of tracks, which is empty if there are no tracks with the media characteristic.

## Discussion

Apple discourages using this method in iOS 15, tvOS 15, macOS 12, and watchOS 8 or later. Load tracks asynchronously using loadTracks(withMediaCharacteristic:completionHandler:) instead.

You can call this method without blocking the current thread when the data in the tracks property is already loaded.

