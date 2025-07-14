

- AVFoundation
- AVFragmentedAsset
-  tracks Deprecated

Instance Property

# tracks

The tracks an asset contains.

iOS 12.0–16.0DeprecatediPadOS 12.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.11–13.0DeprecatedtvOS 12.0–16.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 6.0–9.0Deprecated

``` source
var tracks: [AVFragmentedAssetTrack] { get }
```

Deprecated

Load the value of tracks asynchronously instead.

## See Also

### Accessing Tracks

func track(withTrackID: CMPersistentTrackID) -> AVFragmentedAssetTrack?

Returns a track that contains the specified identifier.

Deprecated

func tracks(withMediaType: AVMediaType) -> [AVFragmentedAssetTrack]

Returns tracks that present media of a specified type.

Deprecated

func tracks(withMediaCharacteristic: AVMediaCharacteristic) -> [AVFragmentedAssetTrack]

Returns tracks that present media of a specified characteristic.

Deprecated

