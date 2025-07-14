

- Apple Music Feed
- Album
-  Album.ReleaseDate 

Object

# Album.ReleaseDate

A mapping of locale to release date for the album.

AppleMusicFeed 1.0+

``` source
object Album.ReleaseDate
```

## Properties

`locale`

`string`

A locale in the IETF language tag format. An empty value indicates fallback to `default`.

`releaseDate`

`string`

The date of content release in YYYY-MM-DD format. For Apple Music, the locale is always `default`, so the release date is the same regardless of the time zone.

## Attributes 

Possible types:

## See Also

### Related objects

object Album.ArtistRole

Information about an artist’s role.

object Album.Artworks

A mapping of locale to localized album cover art.

object Album.Genre

A genre name and its structure.

object Album.Name

A mapping of locale to localized names for the album.

object Album.NamePronunciation

A mapping of locale to translations for the specific pronunciation-name translation type.

object Album.Prices

A mapping of locale to pricing information.

object Album.RecordLabel

Information about a record label.

object Album.RelatedArtist

Information about a related artist.

object Album.RelatedSong

Information about a related song.

object Album.TitleVersion

A mapping of locale to translations for the specific title-version translation type.

object Album.TitleVersionPronunciation

A mapping of locale to translations for the specific title-version-pronunciation-name translation type.

