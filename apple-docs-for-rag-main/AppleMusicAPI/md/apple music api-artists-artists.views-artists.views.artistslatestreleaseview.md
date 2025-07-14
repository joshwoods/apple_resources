

- Apple Music API
- Artists
- Artists.Views
-  Artists.Views.ArtistsLatestReleaseView 

Object

# Artists.Views.ArtistsLatestReleaseView

A relationship view from this artist to the latest release for the artist determined to still be recent by the Apple Music Catalog.

Apple Music 1.0+

``` source
object Artists.Views.ArtistsLatestReleaseView
```

## Properties

`href`

`string`

A relative location for the view.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the view if more exist.

`attributes`

Artists.Views.ArtistsLatestReleaseView.Attributes

 (Required) 

The attributes for the view.

`data`

`[`Albums`]`

 (Required) 

The latest release for the artist determined to still be recent by the Apple Music Catalog.

## Topics

### Related Objects

object Artists.Views.ArtistsLatestReleaseView.Attributes

The latest release for the artist determined to still be recent by the Apple Music Catalog.

## See Also

### Related Objects

object Artists.Views.ArtistsAppearsOnAlbumsView

A relationship view from this artist to a selection of albums from other artists on which this artist also appears.

object Artists.Views.ArtistsCompilationAlbumsView

A relationship view from this artist to albums associated with the artist categorized as compilations.

object Artists.Views.ArtistsFeaturedAlbumsView

A relationship view from this artist to a collection of albums selected as featured for the artist.

object Artists.Views.ArtistsFeaturedMusicVideosView

A relationship view from this artist to a collection of music videos selected as featured for the artist.

object Artists.Views.ArtistsFeaturedPlaylistsView

A relationship view from this artist to relevant playlists associated with the artist.

object Artists.Views.ArtistsFullAlbumsView

A relationship view from this artist to full-release albums associated with the artist.

object Artists.Views.ArtistsLiveAlbumsView

A relationship view from this artist to albums associated with the artist categorized as live performances.

object Artists.Views.ArtistsSimilarArtistsView

A relationship view from this artist to other artists similar to this artist.

object Artists.Views.ArtistsSinglesView

A relationship view from this artist to albums associated with the artist categorized as singles.

object Artists.Views.ArtistsTopMusicVideosView

A relationship view from this artist to relevant music videos associated with the artist.

object Artists.Views.ArtistsTopSongsView

A relationship view from this artist to songs associated with the artist based on popularity in the current storefront.

