

- AVFoundation
- AVFragmentedAsset
-  track(withTrackID:) Deprecated

Instance Method

# track(withTrackID:)

Returns a track that contains the specified identifier.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedtvOS 9.0–16.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
func track(withTrackID trackID: CMPersistentTrackID) -> AVFragmentedAssetTrack?
```

Deprecated

Use loadTrack(withTrackID:completionHandler:) instead.

## Parameters 

`trackID`  

The identifier of the track to return.

## Return Value

A fragmented asset track, or `nil` if no track with the specified identifier is available.

## Discussion

Apple discourages the use of this method in iOS 15, tvOS 15, and macOS 12 or later. Load a track asynchronously using loadTrack(withTrackID:completionHandler:) instead.

You may call this method without blocking the current thread after you’ve asynchronously loaded the tracks property.

## See Also

### Accessing Tracks

var tracks: [AVFragmentedAssetTrack]

The tracks an asset contains.

Deprecated

func tracks(withMediaType: AVMediaType) -> [AVFragmentedAssetTrack]

Returns tracks that present media of a specified type.

Deprecated

func tracks(withMediaCharacteristic: AVMediaCharacteristic) -> [AVFragmentedAssetTrack]

Returns tracks that present media of a specified characteristic.

Deprecated

