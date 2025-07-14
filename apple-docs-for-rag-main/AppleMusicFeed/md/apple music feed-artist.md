

- Apple Music Feed
-  Artist 

Object

# Artist

The data structure that represents an Artist resource.

AppleMusicFeed 1.0+

``` source
object Artist
```

## Properties

`artistType`

`string`

The artist type for the artist. The possible values are `artist`, `tv-show`, `studio`, `podcast-artist`, `author`, `movie-artist`, `software-artist`, `itunes-u-artist`, and `trainer`.

`id`

`string`

The identifier for the artist in Apple Music.

`lastModifiedTime`

`string`

The time, in ISO 8601 format, of the entity’s most recent update.

`name`

Artist.Name

**(Required)** A mapping of locale to localized uncensored names for the artist.

`nameDefault`

`string`

The default name for the artist.

`namePronunciation`

Artist.NamePronunciation

**(Required)** A mapping of locale to translations for the specific pronunciation-name translation type.

`urlTemplate`

`string`

A template for the URL to view the entity in Apple Music. The template requires an ISO country code for the `{country-code}` placeholder.

## Attributes 

Possible types:

## Topics

### Related objects

object Artist.Name

A mapping of locale to localized names for the artist.

object Artist.NamePronunciation

A mapping of locale to translations for the specific pronunciation-name translation type.

## See Also

### Objects

object Album

The data structure that represents an Album resource.

object Song

The data structure that represents a Song resource.

object PopularityTopChartAlbums

The data structure that represents an album popularity chart resource.

object PopularityTopChartSongs

The data structure that represents a song popularity chart resource.

