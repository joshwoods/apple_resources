

- MusicKit
-  MusicLibraryRequest 

Structure

# MusicLibraryRequest

A request that your app uses to fetch items from the user’s music library.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 14.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct MusicLibraryRequest where MusicItemType : MusicLibraryRequestable
```

## Topics

### Initializers

init()

Creates a request to fetch items from the library.

### Instance Properties

var includeOnlyDownloadedContent: Bool

A Boolean value that indicates whether the library response should only include items downloaded on the user’s device.

var limit: Int

A limit for the number of items to return in the library response.

var offset: Int

An offset for the request.

### Instance Methods

func filter(matching: KeyPath&lt;MusicItemType.LibraryFilter, String?>, contains: String)

Filters items by a given optional property that contains a specific string.

func filter(matching: KeyPath&lt;MusicItemType.LibraryFilter, String>, contains: String)

Filters items by a given property that contains a specific string.

func filter&lt;RelatedMusicItemType>(matching: KeyPath&lt;MusicItemType.LibraryFilter, MusicItemCollection&lt;RelatedMusicItemType>?>, contains: RelatedMusicItemType)

Filters items by a given relationship that matches a specific value.

func filter&lt;Value>(matching: KeyPath&lt;MusicItemType.LibraryFilter, Value>, equalTo: Value)

Filters items by a given property that matches a specific value.

func filter&lt;Value>(matching: KeyPath&lt;MusicItemType.LibraryFilter, Value?>, equalTo: Value?)

Filters items by a given optional property that matches a specific value.

func filter&lt;Value>(matching: KeyPath&lt;MusicItemType.LibraryFilter, Value?>, memberOf: [Value?])

Filters items by an optional property for an array of possible values.

func filter&lt;Value>(matching: KeyPath&lt;MusicItemType.LibraryFilter, Value>, memberOf: [Value])

Filters items by a property for an array of possible values.

func filter(text: String)

Filters items by a specific string.

func response() async throws -> MusicLibraryResponse&lt;MusicItemType>

Fetches items from the user’s music library.

func sort&lt;Value>(by: KeyPath&lt;MusicItemType.LibrarySortProperties, Value>, ascending: Bool)

Sorts items by a specified property.

