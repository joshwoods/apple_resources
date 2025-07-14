

- AVFoundation
-  AVFragmentMinding 

Protocol

# AVFragmentMinding

A protocol that defines whether an asset supports fragment minding.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol AVFragmentMinding
```

## Topics

### Fragment Minder Association

var isAssociatedWithFragmentMinder: Bool

A Boolean value that indicates whether an asset that supports fragment minding is currently associated with a fragment minder.

**Required**

## Relationships

### Conforming Types

- AVFragmentedAsset
- AVFragmentedMovie

## See Also

### Fragmented assets

class AVFragmentedAsset

An asset with a duration that the system can extend without modifying its existing media data.

class AVFragmentedAssetTrack

An object that provides the track-level interface to inspect a fragmented asset’s media tracks.

class AVFragmentedAssetMinder

An object that periodically checks whether the system adds new fragments to a fragmented asset.

