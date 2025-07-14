

- Apple Music Feed
- Album
-  Album.Prices 

Object

# Album.Prices

A mapping of locale to pricing information.

AppleMusicFeed 1.0+

``` source
object Album.Prices
```

## Properties

`prices`

`[`Album.Prices.Price`]`

A list of localized pricing information for the content.

`storefront`

`string`

## Attributes 

Possible types:

## Data example

The feed export is in Parquet format. This data example is in JSON format for illustrative purposes.

```
{
"prices": {
    "fr": [
        {
            "currencyCode": "EUR",
            "price": "1.29",
            "priceType": "buy"
            "quality": "standard-definition"
        },
        {
            "currencyCode": "EUR",
            "price": "2.29",
            "priceType": "buy"
            "quality": "high-definition"
        }
    ]
}
}
```

## Topics

### Related objects

object Album.Prices.Price

Information about a pricing offer.

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

