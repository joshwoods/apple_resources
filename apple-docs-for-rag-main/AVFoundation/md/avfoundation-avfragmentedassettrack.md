

- AVFoundation
-  AVFragmentedAssetTrack 

Class

# AVFragmentedAssetTrack

An object that provides the track-level interface to inspect a fragmented asset’s media tracks.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.11+tvOS 12.0+visionOS 1.0+watchOS 6.0+

``` source
class AVFragmentedAssetTrack
```

## Overview

This class subclasses AVAssetTrack. It has no methods or properties of its own.

## Relationships

### Inherits From

- AVAssetTrack

### Conforms To

- AVAsynchronousKeyValueLoading
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Fragmented assets

class AVFragmentedAsset

An asset with a duration that the system can extend without modifying its existing media data.

class AVFragmentedAssetMinder

An object that periodically checks whether the system adds new fragments to a fragmented asset.

protocol AVFragmentMinding

A protocol that defines whether an asset supports fragment minding.

