

- Apple Music API
- Stations
-  Stations.Attributes 

Object

# Stations.Attributes

The attributes for a station resource.

Apple Music 1.0+

``` source
object Stations.Attributes
```

## Properties

`artwork`

Artwork

 (Required) 

The radio station artwork.

`durationInMillis`

`integer`

The duration of the stream. This value isn’t emitted for ‘live’ or programmed stations.

`editorialNotes`

EditorialNotes

The notes about the station that appear in Apple Music.

`episodeNumber`

`string`

The episode number of the station. This value appears when the station represents an episode of a show or other content.

`contentRating`

`string`

The rating of the content possibly heard while playing the station. The possible values for this rating are `clean` and `explicit`. No value means no rating.

Possible Values: `clean, explicit`

`isLive`

`boolean`

 (Required) 

Indicates whether the station is a livestream.

`mediaKind`

`string`

 (Required) 

The media kind for the station. It can have value `audio` or `video` depending on whether it has video stream or audio stream.

Possible Values: `audio, video`

`name`

`string`

 (Required) 

The localized name of the station.

`playParams`

PlayParameters

When present, this attribute indicates that the radio station or episode is available to play with an Apple Music subscription. The value map may be used to initiate playback of the station. Live radio stations and episodes initiate streaming playback. Track-based stations initiate playback of individual tracks.

`stationProviderName`

`string`

The name of the entity that provided the station, when specified.

`url`

`string`

 (Required) 

The URL for sharing the station in Apple Music.

## See Also

### Related Objects

object Stations.Relationships

The name of the relationship you want to fetch for this resource.

