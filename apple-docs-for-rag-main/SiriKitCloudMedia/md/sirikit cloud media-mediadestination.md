

- SiriKit Cloud Media
-  MediaDestination 

Object

# MediaDestination

The user’s library or a playlist.

SiriKit Cloud Media 1.0.2+

``` source
object MediaDestination
```

## Properties

`mediaDestinationType`

`string`

 (Required) 

The type of collection the user wants to store their media items in.

Possible Values: `library, playlist`

## Discussion

A playlist can be either a MediaItem or a MediaDestination. When the user adds a song to a playlist, the playlist is the MediaDestination. When the user adds a playlist to their library, the playlist is a MediaItem, and the user’s library is the MediaDestination.

## Relationships

### Inherited By

- MediaDestinationLibrary
- MediaDestinationPlaylist

## See Also

### Providing a Destination

object AddMediaMediaDestinationResolutionResult.Success

A media destination that successfully matches an intent.

object MediaDestinationLibrary

The user’s library as a destination for an add media intent.

object MediaDestinationPlaylist

A playlist as a destination for an add media intent.

