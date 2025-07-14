

- MusicKit
-  MusicCatalogResourceRequest 

Structure

# MusicCatalogResourceRequest

A request that your app uses to fetch items from the Apple Music catalog using a filter.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct MusicCatalogResourceRequest where MusicItemType : MusicItem, MusicItemType : Decodable
```

## Topics

### Initializers

init()

Creates a request to fetch top-level items in the Apple Music catalog.

init&lt;Value>(matching: KeyPath&lt;MusicItemType.FilterType, Value>, equalTo: Value)

Creates a request to fetch items using a filter that matches a specific value.

init&lt;Value>(matching: KeyPath&lt;MusicItemType.FilterType, Value>, memberOf: [Value])

Creates a request to fetch items using a filter that matches any value from an array of possible values.

### Instance Properties

var limit: Int?

A limit for the number of items to return in the catalog resource response.

var properties: [PartialMusicAsyncProperty&lt;MusicItemType>]

A list of properties which the resource request will fetch for each music item in the response.

### Instance Methods

func response() async throws -> MusicCatalogResourceResponse&lt;MusicItemType>

Fetches items from the Apple Music catalog that match a specific filter.

## Relationships

### Conforms To

- Sendable

## See Also

### Resource Loading Using Filters

struct MusicCatalogResourceResponse

An object that contains results for a catalog resource request.

protocol AlbumFilter

Album properties your app uses as a filter for a catalog resource request.

protocol ArtistFilter

Artist properties your app uses as a filter for a catalog resource request.

protocol CuratorFilter

Curator properties your app uses as a filter for a catalog resource request.

protocol GenreFilter

Genre properties your app uses as a filter for a catalog resource request.

protocol MusicVideoFilter

Music video properties your app uses as a filter for a catalog resource request.

protocol PlaylistFilter

Playlist properties your app uses as a filter for a catalog resource request.

protocol RadioShowFilter

Radio Show properties your app uses as a filter for a catalog resource request.

protocol RecordLabelFilter

The set of record label properties your app uses as a filter for a catalog resource request.

protocol SongFilter

Song properties your app uses as a filter for a catalog resource request.

protocol StationFilter

The set of station properties your app uses as a filter for a catalog resource request.

protocol FilterableMusicItem

A declaration of the associated type that contains the set of music item properties your app uses as a filter for a catalog resource request.

