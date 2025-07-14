

- Media Player
-  MPMediaPlaylist 

Class

# MPMediaPlaylist

A playable collection of related media items.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class MPMediaPlaylist
```

## Overview

Each playlist has a name, a set of attributes, and a unique identifier that persists across application launches.

Users configure playlists using iTunes or by creating a playlist on the device. Playlists are read-only to your iOS app. To obtain playlists, configure a media query that’s grouped by playlist. Each returned media item collection is a media playlist. The following code snippet illustrates this by logging playlist and song names to the Xcode debugger console:

- Swift
- Objective-C

```
let myPlaylistQuery = MPMediaQuery.playlists()
let playlists = myPlaylistQuery.collections
for playlist in playlists! {
    print(playlist.value(forProperty: MPMediaPlaylistPropertyName)!)

    let songs = playlist.items
    for song in songs {
        let songTitle = song.value(forProperty: MPMediaItemPropertyTitle)
        print("\t\t", songTitle!)
    }
}
```

```
MPMediaQuery *myPlaylistsQuery = [MPMediaQuery playlistsQuery];
NSArray *playlists = [myPlaylistsQuery collections];

for (MPMediaPlaylist *playlist in playlists) {
    NSLog (@"%@", [playlist valueForProperty: MPMediaPlaylistPropertyName]);

    NSArray *songs = [playlist items];
    for (MPMediaItem *song in songs) {
        NSString *songTitle =
            [song valueForProperty: MPMediaItemPropertyTitle];
        NSLog (@"\t\t%@", songTitle);
    }
}
```

MPMediaPropertyPredicate and MPMediaQuery describe the API for building a media query. MPMediaEntity describes the methods for querying media playlist property values.

## Topics

### Adding media items to a playlist

func addItem(withProductID: String, completionHandler: (((any Error)?) -> Void)?)

Adds the item associated with the product identifier to the end of the playlist.

func add([MPMediaItem], completionHandler: (((any Error)?) -> Void)?)

Adds an array of media items to the end of the playlist.

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

struct MPMediaPlaylistAttribute

Attributes define the type of playlist.

var seedItems: [MPMediaItem]?

The items seeded to generate the playlist; applies only to Genius playlists.

### Property keys

Playlist property keys

Keys that contain information about a playlist.

## Relationships

### Inherits From

- MPMediaItemCollection

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Media items and playlists

class MPMediaItem

A collection of properties that represents a single item in the media library.

class MPMediaItemArtwork

A graphical image, such as music album cover art, associated with a media item.

class MPMediaItemCollection

A sorted set of media items from the media library.

class MPMediaPlaylistCreationMetadata

A set of attributes for describing a playlist when creating it.

class MPMediaEntity

The abstract superclass for media items, media item collections, and media playlist instances.

