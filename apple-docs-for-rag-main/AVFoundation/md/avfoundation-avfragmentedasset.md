

- AVFoundation
-  AVFragmentedAsset 

Class

# AVFragmentedAsset

An asset with a duration that the system can extend without modifying its existing media data.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.11+tvOS 12.0+visionOS 1.0+watchOS 6.0+

``` source
class AVFragmentedAsset
```

## Overview

By using an `mvex` box in their `moov` box, QuickTime movie files and MPEG-4 files can indicate that they accommodate additional fragments. To determine whether a fragmented asset can monitor the addition of fragments, check the value of its canContainFragments property.

Associate a fragmented asset with an instance of AVFragmentedAssetMinder to know when the system appends new fragments. When it has an associated asset minder, AVFragmentedAssetTrack posts AVAssetDurationDidChangeNotification notifications whenever it detects new fragments. It may also post AVAssetContainsFragmentsDidChangeNotification and AVAssetWasDefragmentedNotification, as the documentation of those notifications explains.

## Topics

### Loading Tracks

static var tracks: AVAsyncProperty&lt;Root, [AVFragmentedAssetTrack]>

The tracks an asset contains.

func loadTrack(withTrackID: CMPersistentTrackID, completionHandler: (AVFragmentedAssetTrack?, (any Error)?) -> Void)

Loads a track that contains the specified identifier.

func loadTracks(withMediaType: AVMediaType, completionHandler: ([AVFragmentedAssetTrack]?, (any Error)?) -> Void)

Loads tracks that contain media of a specified type.

func loadTracks(withMediaCharacteristic: AVMediaCharacteristic, completionHandler: ([AVFragmentedAssetTrack]?, (any Error)?) -> Void)

Loads tracks that contain media of a specified characteristic.

### Accessing Tracks

var tracks: [AVFragmentedAssetTrack]

The tracks an asset contains.

Deprecated

func track(withTrackID: CMPersistentTrackID) -> AVFragmentedAssetTrack?

Returns a track that contains the specified identifier.

Deprecated

func tracks(withMediaType: AVMediaType) -> [AVFragmentedAssetTrack]

Returns tracks that present media of a specified type.

Deprecated

func tracks(withMediaCharacteristic: AVMediaCharacteristic) -> [AVFragmentedAssetTrack]

Returns tracks that present media of a specified characteristic.

Deprecated

## Relationships

### Inherits From

- AVURLAsset

### Conforms To

- AVAsynchronousKeyValueLoading
- AVContentKeyRecipient
- AVFragmentMinding
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSItemProviderReading
- NSItemProviderWriting
- NSObjectProtocol
- Sendable

## See Also

### Fragmented assets

class AVFragmentedAssetTrack

An object that provides the track-level interface to inspect a fragmented asset’s media tracks.

class AVFragmentedAssetMinder

An object that periodically checks whether the system adds new fragments to a fragmented asset.

protocol AVFragmentMinding

A protocol that defines whether an asset supports fragment minding.

