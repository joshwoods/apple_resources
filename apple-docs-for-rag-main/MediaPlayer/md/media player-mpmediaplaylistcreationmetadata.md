

- Media Player
-  MPMediaPlaylistCreationMetadata 

Class

# MPMediaPlaylistCreationMetadata

A set of attributes for describing a playlist when creating it.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+visionOS 1.0+

``` source
class MPMediaPlaylistCreationMetadata
```

## Overview

Use this class when creating a new playlist using the getPlaylist(with:creationMetadata:completionHandler:) method. The system adds the metadata to the playlist when you create it, however it ignores the metadata if the playlist already exists.

## Topics

### Creating metadata for a playlist

init(name: String)

Creates a new playlist metadata object with the designated name.

### Metadata for a playlist

var authorDisplayName: String!

App defined display name for the playlist.

var descriptionText: String

The descriptive text for the playlist.

var name: String

The playlist’s displayed name.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Media items and playlists

class MPMediaItem

A collection of properties that represents a single item in the media library.

class MPMediaItemArtwork

A graphical image, such as music album cover art, associated with a media item.

class MPMediaItemCollection

A sorted set of media items from the media library.

class MPMediaPlaylist

A playable collection of related media items.

class MPMediaEntity

The abstract superclass for media items, media item collections, and media playlist instances.

