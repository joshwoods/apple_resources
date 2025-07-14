

- Apple Music Feed
-  PopularityTopChartSongs 

Object

# PopularityTopChartSongs

The data structure that represents a song popularity chart resource.

AppleMusicFeed 1.0+

``` source
object PopularityTopChartSongs
```

## Properties

`genre`

PopularityTopChartSongs.Genre

**(Required)** The chart’s associated genre.

`rankings`

`[`PopularityTopChartSongs.Rankings`]`

**(Required)** A list of song rankings in the chart.

`storefront`

`string`

**(Required)** The chart’s associated storefront.

## Attributes 

Possible types:

## Topics

### Related objects

object PopularityTopChartSongs.Genre

A genre name and its structure.

object PopularityTopChartSongs.Rankings

A song’s ranking in a popularity chart.

## See Also

### Objects

object Album

The data structure that represents an Album resource.

object Song

The data structure that represents a Song resource.

object Artist

The data structure that represents an Artist resource.

object PopularityTopChartAlbums

The data structure that represents an album popularity chart resource.

