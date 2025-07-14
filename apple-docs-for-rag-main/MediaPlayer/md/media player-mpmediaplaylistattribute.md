

- Media Player
-  MPMediaPlaylistAttribute 

Structure

# MPMediaPlaylistAttribute

Attributes define the type of playlist.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
struct MPMediaPlaylistAttribute
```

## Overview

Playlist attributes to use as possible values for the MPMediaPlaylistPropertyPlaylistAttributes property.

## Topics

### Constants

static var onTheGo: MPMediaPlaylistAttribute

A playlist created on a device rather than synced from the Music app.

static var smart: MPMediaPlaylistAttribute

A smart playlist includes items that match one or more user-specified rules.

static var genius: MPMediaPlaylistAttribute

A Genius playlist includes items related to other items in your Music library.

### Initializers

init(rawValue: UInt)

Creates a new instance with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Retrieving information about a playlist

var authorDisplayName: String?

The display name for the playlist defined in the app.

var descriptionText: String?

User supplied text that describes the playlist.

var name: String?

The name of the playlist.

var persistentID: MPMediaEntityPersistentID

The persistent identifier for the playlist.

var cloudGlobalID: String?

The cloud identifier for the playlist.

var playlistAttributes: MPMediaPlaylistAttribute

The attributes associated with the playlist.

var seedItems: [MPMediaItem]?

The items seeded to generate the playlist; applies only to Genius playlists.

