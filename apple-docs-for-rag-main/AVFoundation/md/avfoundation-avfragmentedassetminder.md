

- AVFoundation
-  AVFragmentedAssetMinder 

Class

# AVFragmentedAssetMinder

An object that periodically checks whether the system adds new fragments to a fragmented asset.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.11+tvOS 12.0+visionOS 1.0+watchOS 6.0+

``` source
class AVFragmentedAssetMinder
```

## Topics

### Creating an Asset Minder

init(asset: any AVAsset &amp; AVFragmentMinding, mindingInterval: TimeInterval)

Creates a fragmented asset minder that monitors the specified asset at the indicated minding interval.

### Configuring the Minding Interval

var mindingInterval: TimeInterval

An interval that specifies when to perform a check for additional fragments.

### Inspecting a Fragment Asset

var assets: [any AVAsset &amp; AVFragmentMinding]

The minded array of fragmented assets.

### Adding and Removing Fragmented Assets

func addFragmentedAsset(any AVAsset &amp; AVFragmentMinding)

Adds a fragmented asset to the array of minded assets.

func removeFragmentedAsset(any AVAsset &amp; AVFragmentMinding)

Removes a fragmented asset from the array of minded assets.

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVFragmentedMovieMinder

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Fragmented assets

class AVFragmentedAsset

An asset with a duration that the system can extend without modifying its existing media data.

class AVFragmentedAssetTrack

An object that provides the track-level interface to inspect a fragmented asset’s media tracks.

protocol AVFragmentMinding

A protocol that defines whether an asset supports fragment minding.

