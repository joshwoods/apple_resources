

- MusicKit
-  MusicCatalogSearchRequest 

Structure

# MusicCatalogSearchRequest

A request that your app uses to fetch items from the Apple Music catalog using a search term.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct MusicCatalogSearchRequest
```

## Topics

### Initializers

init(term: String, types: [any MusicCatalogSearchable.Type])

Creates a catalog search request for a specified search term and list of catalog searchable types.

### Instance Properties

var includeTopResults: Bool

A Boolean value that indicates whether to request top search results.

var limit: Int?

A limit for the number of items to return in the catalog search response.

var offset: Int?

An offet for the request.

let term: String

The search term for the request.

var types: [any MusicCatalogSearchable.Type]

The list of requested catalog searchable types.

### Instance Methods

func response() async throws -> MusicCatalogSearchResponse

Fetches items of the requested catalog searchable types that match the search term of the request.

## See Also

### Catalog Search

struct MusicCatalogSearchResponse

An object that contains results for a catalog search request.

protocol MusicCatalogSearchable

A protocol for music items that your app can fetch by using a catalog search request.

