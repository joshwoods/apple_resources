

- Apple Music Feed
- Song
-  Song.ReleaseDate 

Object

# Song.ReleaseDate

A mapping of locale to release date for the song.

AppleMusicFeed 1.0+

``` source
object Song.ReleaseDate
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

object Song.ArtistRole

Information about an artist’s role.

object Song.Genre

A genre name and its structure.

object Song.Name

A mapping of locale to localized names for the song.

object Song.NamePronunciation

A mapping of locale to translations for the specific pronunciation-name translation type.

object Song.Prices

A mapping of locale to pricing information.

object Song.RelatedAlbum

Information about a related album.

object Song.RelatedArtist

Information about a related artist.

object Song.TitleVersion

A mapping of locale to translations for the specific title-version translation type.

object Song.TitleVersionPronunciation

A mapping of locale to translations for the specific title-version-pronunciation-name translation type.

