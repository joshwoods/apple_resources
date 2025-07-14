

- Apple Music Feed
- Song
-  Song.Prices 

Object

# Song.Prices

A mapping of locale to pricing information.

AppleMusicFeed 1.0+

``` source
object Song.Prices
```

## Properties

`prices`

`[`Song.Prices.Price`]`

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

object Song.Prices.Price

Information about a pricing offer.

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

