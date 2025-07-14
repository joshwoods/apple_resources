

- Apple Music Feed
- Song
-  Song.Genre 

Object

# Song.Genre

A genre name and its structure.

AppleMusicFeed 1.0+

``` source
object Song.Genre
```

## Properties

`name`

`string`

The name of the genre.

`path`

`[string]`

A list of genres in hierarchical order. For example, if `Classical` is a subgenre of `Music`, this value is `[‘Music’, ‘Classical’]`.

## Attributes 

Possible types:

## Discussion

Genres are hierarchical beginning with the genre `Music`.

## Data example

The feed export is in Parquet format. This data example is in JSON format for illustrative purposes.

```
{
    "genres": {
        "name": "Rock",
        "path": [
            "Music",
            "Classical",
            "Rock"
        ]
    }
}
```

## See Also

### Related objects

object Song.ArtistRole

Information about an artist’s role.

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

