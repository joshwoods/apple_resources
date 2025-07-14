

- Apple Music API
- ChartResponse
- ChartResponse.Results
-  ChartResponse.Results.SongsChart 

Object

# ChartResponse.Results.SongsChart

The songs results of a chart.

Apple Music 1.0+

``` source
object ChartResponse.Results.SongsChart
```

## Properties

`chart`

`string`

 (Required) 

The unique name of the chart to use when fetching a specific chart.

`data`

`[`Songs`]`

 (Required) 

The popularity-ordered songs for the chart.

`href`

`string`

A relative location to fetch the chart results directly.

`name`

`string`

 (Required) 

The localized display name for the chart.

`next`

`string`

A relative cursor to fetch the next paginated results for the chart if more exist.

## See Also

### Related Objects

object ChartResponse.Results.AlbumsChart

The albums results of a chart.

object ChartResponse.Results.MusicVideosChart

The music videos results of a chart.

object ChartResponse.Results.PlaylistsChart

The playlists results of a chart.

