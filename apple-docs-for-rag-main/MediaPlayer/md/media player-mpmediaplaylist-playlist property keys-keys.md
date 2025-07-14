

- Media Player
- MPMediaPlaylist
-  Playlist property keys 

API Collection

# Playlist property keys

Keys that contain information about a playlist.

## Overview

Use these keys with the canFilter(byProperty:) and value(forProperty:) methods to obtain information about a playlist. You can use properties described as “filterable” to build media property predicates (see MPMediaPropertyPredicate).

## Topics

### Property keys

let MPMediaPlaylistPropertyAuthorDisplayName: String

App defined name for the playlist.

let MPMediaPlaylistPropertyName: String

The name of the playlist.

let MPMediaPlaylistPropertyDescriptionText: String

Descriptive text for the playlist.

let MPMediaPlaylistPropertyPersistentID: String

The persistent identifier for the playlist.

let MPMediaPlaylistPropertyPlaylistAttributes: String

The attributes associated with the playlist.

let MPMediaPlaylistPropertyCloudGlobalID: String

The cloud identifier for the playlist.

let MPMediaPlaylistPropertySeedItems: String

The items seeded to generate the playlist; applies only to Genius playlists.

