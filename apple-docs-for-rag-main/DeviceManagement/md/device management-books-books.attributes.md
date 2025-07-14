

- Device Management
- Books
-  Books.Attributes 

Object

# Books.Attributes

The attributes for a books resource.

Device Assignment ServicesVPP License Management

``` source
object Books.Attributes
```

## Properties

`artistName`

`string`

 (Required) 

The name of the artist for this content.

`artwork`

Artwork

 (Required) 

The artwork for this content.

`genreNames`

`[string]`

 (Required) 

A list of genre names associated with this content.

`isbn`

`string`

The ISBN of this book.

`name`

`string`

 (Required) 

The (potentially) censored name of the content.

`offers`

`[`Books.Attributes.Offers`]`

 (Required) 

A map of offer and asset information for the associated content.

`seriesInfo`

Books.Attributes.SeriesInfo

Info about the series this book is a part of.

`taxExclusivePrices`

`[`Books.Attributes.TaxExclusivePrices`]`

**(Personalized)** Tax-exclusive prices for this salable.

`taxRate`

`number`

**(Personalized)** Tax rate for this salable for the current account.

`url`

`string`

 (Required) 

A canonical URL to the content that may be used for sharing or linking to the content externally.

`userRating`

Books.Attributes.UserRating

 (Required) 

User rating information for the content.

## Topics

### Related Objects

object Books.Attributes.Offers

object Books.Attributes.SeriesInfo

object Books.Attributes.TaxExclusivePrices

object Books.Attributes.UserRating

## See Also

### Related Objects

object Books.Relationships

