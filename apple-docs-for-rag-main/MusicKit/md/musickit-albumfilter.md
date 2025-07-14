

- MusicKit
-  AlbumFilter 

Protocol

# AlbumFilter

Album properties your app uses as a filter for a catalog resource request.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
protocol AlbumFilter
```

## Topics

### Instance Properties

var id: MusicItemID

The unique identifier for the album.

**Required**

var upc: String?

The universal product code (UPC) for the album.

**Required**

## See Also

### Resource Loading Using Filters

struct MusicCatalogResourceRequest

A request that your app uses to fetch items from the Apple Music catalog using a filter.

struct MusicCatalogResourceResponse

An object that contains results for a catalog resource request.

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

