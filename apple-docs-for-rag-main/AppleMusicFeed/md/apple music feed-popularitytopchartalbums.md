

- Apple Music Feed
-  PopularityTopChartAlbums 

Object

# PopularityTopChartAlbums

The data structure that represents an album popularity chart resource.

AppleMusicFeed 1.0+

``` source
object PopularityTopChartAlbums
```

## Properties

`genre`

PopularityTopChartAlbums.Genre

**(Required)** The chart’s associated genre.

`rankings`

`[`PopularityTopChartAlbums.Rankings`]`

**(Required)** A list of album rankings in the chart.

`storefront`

`string`

**(Required)** The chart’s associated storefront.

## Attributes 

Possible types:

## Topics

### Related objects

object PopularityTopChartAlbums.Genre

A genre name and its structure.

object PopularityTopChartAlbums.Rankings

An album’s ranking in a popularity chart.

## See Also

### Objects

object Album

The data structure that represents an Album resource.

object Song

The data structure that represents a Song resource.

object Artist

The data structure that represents an Artist resource.

object PopularityTopChartSongs

The data structure that represents a song popularity chart resource.

