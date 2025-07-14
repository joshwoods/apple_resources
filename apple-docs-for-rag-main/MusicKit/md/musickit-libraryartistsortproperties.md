

- MusicKit
-  LibraryArtistSortProperties 

Protocol

# LibraryArtistSortProperties

Artist properties your app uses to sort results for a library request.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 14.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol LibraryArtistSortProperties
```

## Topics

### Instance Properties

var albumCount: Int?

The number of albums from this artist.

**Required**

var libraryAddedDate: Date?

The date when the user added the artist to the library.

**Required**

var name: String

The name of the artist.

**Required**

