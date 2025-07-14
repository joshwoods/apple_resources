

- AVFoundation
- AVFragmentedAsset
-  tracks(withMediaType:) Deprecated

Instance Method

# tracks(withMediaType:)

Returns tracks that present media of a specified type.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedtvOS 9.0–16.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
func tracks(withMediaType mediaType: AVMediaType) -> [AVFragmentedAssetTrack]
```

Deprecated

Use loadTracks(withMediaType:completionHandler:) instead.

## Parameters 

`mediaType`  

The media type according to which the asset filters its tracks. For valid values see AVMediaType.

## Return Value

An array of tracks of a specific media characteristic.

## Discussion

Apple discourages the use of this method in iOS 15, tvOS 15, and macOS 12 or later. Load tracks asynchronously using loadTracks(withMediaType:completionHandler:) instead.

You may call this method without blocking the current thread after you’ve asynchronously loaded the tracks property.

## See Also

### Accessing Tracks

var tracks: [AVFragmentedAssetTrack]

The tracks an asset contains.

Deprecated

func track(withTrackID: CMPersistentTrackID) -> AVFragmentedAssetTrack?

Returns a track that contains the specified identifier.

Deprecated

func tracks(withMediaCharacteristic: AVMediaCharacteristic) -> [AVFragmentedAssetTrack]

Returns tracks that present media of a specified characteristic.

Deprecated

