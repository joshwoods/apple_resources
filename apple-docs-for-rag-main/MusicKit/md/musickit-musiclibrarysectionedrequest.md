

- MusicKit
-  MusicLibrarySectionedRequest 

Structure

# MusicLibrarySectionedRequest

A request that your app uses to fetch items grouped by sections from the user’s music library.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 14.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct MusicLibrarySectionedRequest where SectionType : MusicLibrarySectionRequestable, MusicItemType : MusicLibraryRequestable
```

## Topics

### Initializers

init()

Creates a request to fetch items grouped by sections from the library.

### Instance Properties

var includeOnlyDownloadedContent: Bool

A Boolean value that indicates whether the library response should only include items downloaded on the user’s device.

var limit: Int

A limit for the number of items to return in the library response.

var offset: Int

An offset for the request.

### Instance Methods

func filterItems&lt;RelatedMusicItemType>(matching: KeyPath&lt;MusicItemType.LibraryFilter, MusicItemCollection&lt;RelatedMusicItemType>?>, contains: RelatedMusicItemType)

Filters items by a given relationship that matches a specific value.

func filterItems(matching: KeyPath&lt;MusicItemType.LibraryFilter, String>, contains: String)

Filters items by a given property that contains a specific string.

func filterItems(matching: KeyPath&lt;MusicItemType.LibraryFilter, String?>, contains: String)

Filters items by a given optional property that contains a specific string.

func filterItems&lt;Value>(matching: KeyPath&lt;MusicItemType.LibraryFilter, Value>, equalTo: Value)

Filters items by a given property that matches a specific value.

func filterItems&lt;Value>(matching: KeyPath&lt;MusicItemType.LibraryFilter, Value?>, equalTo: Value?)

Filters items by a given optional property that matches a specific value.

func filterItems&lt;Value>(matching: KeyPath&lt;MusicItemType.LibraryFilter, Value>, memberOf: [Value])

Filters items by a property for an array of possible values.

func filterItems&lt;Value>(matching: KeyPath&lt;MusicItemType.LibraryFilter, Value?>, memberOf: [Value?])

Filters items by an optional property for an array of possible values.

func filterItems(text: String)

Filters items by a specific string.

func filterSections(matching: KeyPath&lt;SectionType.LibraryFilter, String?>, contains: String)

Filters sections by a given optional property that contains a specific string.

func filterSections(matching: KeyPath&lt;SectionType.LibraryFilter, String>, contains: String)

Filters sections by a given property that contains a specific string.

func filterSections&lt;Value>(matching: KeyPath&lt;SectionType.LibraryFilter, Value?>, equalTo: Value?)

Filters sections by a given optional property that matches a specific value.

func filterSections&lt;Value>(matching: KeyPath&lt;SectionType.LibraryFilter, Value>, equalTo: Value)

Filters sections by a given property that matches a specific value.

func filterSections&lt;Value>(matching: KeyPath&lt;SectionType.LibraryFilter, Value>, memberOf: [Value])

Filters sections by a property for an array of possible values.

func filterSections&lt;Value>(matching: KeyPath&lt;SectionType.LibraryFilter, Value?>, memberOf: [Value?])

Filters sections by an optional property for an array of possible values.

func filterSections(text: String)

Filters sections by a specific string.

func response() async throws -> MusicLibrarySectionedResponse&lt;SectionType, MusicItemType>

Fetches items grouped by sections from the user’s music library.

func sortItems&lt;Value>(by: KeyPath&lt;MusicItemType.LibrarySortProperties, Value>, ascending: Bool)

Sorts items by a specified property.

func sortSections&lt;Value>(by: KeyPath&lt;SectionType.LibrarySortProperties, Value>, ascending: Bool)

Sorts sections by a specified property.

