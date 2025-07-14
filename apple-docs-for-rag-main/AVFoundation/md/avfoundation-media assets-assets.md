

- AVFoundation
-  Media assets 

API Collection

# Media assets

Load media assets from files and streams to inspect their attributes, tracks, and embedded metadata.

## Topics

### Essentials

Loading media data asynchronously

Build responsive apps by using language-level concurrency features to efficiently load media data.

### Assets

class AVAsset

An object that models timed audiovisual media.

class AVURLAsset

An asset that represents media at a local or remote URL.

class AVAssetTrack

An object that models a track of media that an asset contains.

class AVAssetTrackSegment

An object that represents a time range segment of an asset track.

class AVAssetTrackGroup

A group of related tracks in an asset.

### Metadata

Retrieving media metadata

Load descriptive metadata for media assets and their tracks.

class AVMetadataItem

A metadata item for an audiovisual asset or one of its tracks.

class AVMutableMetadataItem

A mutable metadata item for an audiovisual asset or for one of its tracks.

struct AVMetadataIdentifier

A structure that defines identifiers for metadata formats.

struct AVMetadataKey

A structure that defines a metadata key.

struct AVMetadataKeySpace

A structure that defines a metadata key space.

struct AVMetadataExtraAttributeKey

A structure that defines keys for extra metadata attributes.

struct AVMetadataFormat

A structure that defines metadata formats.

class AVMetadataItemFilter

An object that filters selected information from a metadata item.

### Property loading

protocol AVAsynchronousKeyValueLoading

A protocol that defines the interface to load media data asynchronously.

class AVAsyncProperty

An asynchronous property that constrains its type and value.

class AVPartialAsyncProperty

An asynchronous property that constrains its type.

class AVAnyAsyncProperty

A base class for asynchronous properties.

### Fragmented assets

class AVFragmentedAsset

An asset with a duration that the system can extend without modifying its existing media data.

class AVFragmentedAssetTrack

An object that provides the track-level interface to inspect a fragmented asset’s media tracks.

class AVFragmentedAssetMinder

An object that periodically checks whether the system adds new fragments to a fragmented asset.

protocol AVFragmentMinding

A protocol that defines whether an asset supports fragment minding.

## See Also

### Common

Media reading and writing

Read images from video, export to alternative formats, and perform sample-level reading and writing of media data.

Media types and utilities

Identify the types of content and file formats that AVFoundation supports.

Video settings

Configure video processing settings using standard key and value constants.

Audio settings

Configure audio processing settings using standard key and value constants.

