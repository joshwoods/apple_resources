

- Apple Music Feed
-  Song 

Object

# Song

The data structure that represents a Song resource.

AppleMusicFeed 1.0+

``` source
object Song
```

## Properties

`album`

`[`Song.RelatedAlbum`]`

A list of albums that contain the song.

`artistRoles`

`[`Song.ArtistRole`]`

**(Required)** A list of artists and their roles.

`audioLocale`

`string`

The locale of the audio. This usually corresponds to the language of the song. The locale uses the IETF language tag format.

`contentTraits`

`[string]`

**(Required)** A list of the content traits for the song. The possible values are `remix`, `live`, `compilation`, and `karaoke`.

`copyright`

`string`

The copyright notice text.

`copyrightPline`

`string`

The copyright performance rights text that displays in Apple Music.

`durationInMillis`

`number`

The length of the song in milliseconds.

`featuredArtists`

`[`Song.RelatedArtist`]`

**(Required)** A list of the featured artists of the song.

`genres`

`[`Song.Genre`]`

**(Required)** A list of genre information for the song.

`id`

`string`

The identifier for the song in Apple Music.

`isrc`

`string`

The International Standard Recording Code (ISRC) for the sound or music video recording.

`lastModifiedTime`

`string`

The time, in ISO 8601 format, of the entity’s most recent update.

`name`

Song.Name

**(Required)** A mapping of locale to localized uncensored names for the song.

`nameDefault`

`string`

The default name for the song.

`namePronunciation`

Song.NamePronunciation

**(Required)** A mapping of locale to translations for the specific pronunciation-name translation type.

`parentalAdvisoryType`

`string`

The type of parental advisory status. The possible values are `none`, `explicit`, `not explicit`, and `cleaned`.

`prices`

Song.Prices

**(Required)** A mapping of locale to pricing information. Pricing offer parameters include `price`, `priceType`, and `quality`.

`primaryArtists`

`[`Song.RelatedArtist`]`

**(Required)** A list of the primary artists of the song.

`releaseDate`

Song.ReleaseDate

**(Required)** A mapping of locale to release date, in YYYY-MM-DD format.

`shortPreview`

`string`

**(Required)** A template for the URL for a short audio preview of the song.

`titleVersion`

Song.TitleVersion

**(Required)** A mapping of locale to translations for the specific title-version translation type.

`titleVersionPronunciation`

Song.TitleVersionPronunciation

**(Required)** A mapping of locale to translations for the specific title-version-pronunciation-name translation type.

`trackNumber`

`number`

The track number of the song.

`urlTemplate`

`string`

A template for the URL to view the entity in Apple Music. The template requires an ISO country code for the `{country-code}` placeholder.

`volumeNumber`

`number`

The volume number of the song.

## Attributes 

Possible types:

## Topics

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

object Song.ReleaseDate

A mapping of locale to release date for the song.

object Song.TitleVersion

A mapping of locale to translations for the specific title-version translation type.

object Song.TitleVersionPronunciation

A mapping of locale to translations for the specific title-version-pronunciation-name translation type.

## See Also

### Objects

object Album

The data structure that represents an Album resource.

object Artist

The data structure that represents an Artist resource.

object PopularityTopChartAlbums

The data structure that represents an album popularity chart resource.

object PopularityTopChartSongs

The data structure that represents a song popularity chart resource.

