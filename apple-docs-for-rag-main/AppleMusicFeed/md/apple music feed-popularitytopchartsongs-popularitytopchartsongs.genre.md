

- Apple Music Feed
- PopularityTopChartSongs
-  PopularityTopChartSongs.Genre 

Object

# PopularityTopChartSongs.Genre

A genre name and its structure.

AppleMusicFeed 1.0+

``` source
object PopularityTopChartSongs.Genre
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

object PopularityTopChartSongs.Rankings

A song’s ranking in a popularity chart.

