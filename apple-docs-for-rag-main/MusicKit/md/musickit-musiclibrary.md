

- MusicKit
-  MusicLibrary 

Class

# MusicLibrary

An object your app uses to access the user’s music library.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 14.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
class MusicLibrary
```

## Topics

### Instance Methods

func add&lt;MusicItemType>(MusicItemType) async throws

Adds an item to the user’s music library.

func add&lt;MusicItemType>(MusicItemType, to: Playlist) async throws -> Playlist

Adds an item to the end of an existing playlist.

func createPlaylist(name: String, description: String?, authorDisplayName: String?) async throws -> Playlist

Creates a playlist in the user’s music library.

func createPlaylist&lt;S, MusicPlaylistAddableType>(name: String, description: String?, authorDisplayName: String?, items: S) async throws -> Playlist

Creates a playlist in the user’s music library.

func edit(Playlist, name: String?, description: String?, authorDisplayName: String?) async throws -> Playlist

Edits a playlist that your app has created.

func edit&lt;S, MusicPlaylistAddableType>(Playlist, name: String?, description: String?, authorDisplayName: String?, items: S) async throws -> Playlist

Edits a playlist that your app has created including items to rebuild the list of entries.

### Type Properties

static let shared: MusicLibrary

A shared object that allows your app to modify the user’s music library.

### Enumerations

enum Error

An error that the music library can throw upon accessing, manipulating, or requesting data from the user’s music library.

