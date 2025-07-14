

- Apple Music Feed
- Album
-  Album.Genre 

Object

# Album.Genre

A genre name and its structure.

AppleMusicFeed 1.0+

``` source
object Album.Genre
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

object Album.ArtistRole

Information about an artist’s role.

object Album.Artworks

A mapping of locale to localized album cover art.

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

object Album.ReleaseDate

A mapping of locale to release date for the album.

object Album.TitleVersion

A mapping of locale to translations for the specific title-version translation type.

object Album.TitleVersionPronunciation

A mapping of locale to translations for the specific title-version-pronunciation-name translation type.

