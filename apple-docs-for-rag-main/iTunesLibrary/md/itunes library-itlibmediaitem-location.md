

- iTunes Library
- ITLibMediaItem
-  location 

Instance Property

# location

The location of the media item on disk.

Mac Catalyst 14.0+macOS 10.13+

``` source
var location: URL? { get }
```

## Discussion

If the location of the media item isn’t available, this property returns ITLibMediaItemLocationType.unknown.

This method returns URLs that are outside of the default sandbox. To use the iTunesLibrary framework, a sandboxed app must have the com.apple.security.assets.music.read-write or com.apple.security.assets.music.read-only entitlement.

To access the media item file in a sandboxed app, call startAccessingSecurityScopedResource().

Listing 1.

```
```

For more information about using URLs that are outside the default sandbox from a sandboxed app, see Security-Scoped Bookmarks and Persistent Resource Access.

In nonsandboxed apps, you can use the returned location URL to access the media item file directly.

## See Also

### Getting Media Item Info

var title: String

The title of the media item.

var sortTitle: String?

The title of the media item to use when sorting.

var artist: ITLibArtist?

Information about the artist that iTunes associates with the media item.

var composer: String

The name of the composer that iTunes associates with the media item.

var sortComposer: String?

The name to use when sorting by composer.

var rating: Int

The rating of the media item.

var isRatingComputed: Bool

A Boolean value that indicates whether iTunes computes the media item’s rating from its album rating.

var startTime: Int

If nonzero, the actual time playback of the media item starts instead of 0:00 (in milliseconds).

var stopTime: Int

If nonzero, the actual time playback of the media item stops versus the total time (in milliseconds).

var album: ITLibAlbum

The album of the media item.

var genre: String

The genre of the media item, if any.

var kind: String?

The kind of media item file, such as an MPEG audio file.

var mediaKind: ITLibMediaItemMediaKind

The kind of media item.

var totalTime: Int

The length of the media item in milliseconds.

var trackNumber: Int

The position of the media item within its album.

