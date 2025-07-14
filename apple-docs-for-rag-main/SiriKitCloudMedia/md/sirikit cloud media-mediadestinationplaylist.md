

- SiriKit Cloud Media
-  MediaDestinationPlaylist 

Object

# MediaDestinationPlaylist

A playlist as a destination for an add media intent.

SiriKit Cloud Media 1.0.2+

``` source
object MediaDestinationPlaylist
```

## Properties

`mediaDestinationType`

`string`

 (Required) 

The type of collection the user wants to store their media items in.

Value: `playlist`

`playlistName`

`string`

 (Required) 

The name of the playlist.

Minimum length: `1`

Maximum length: `1000`

## Relationships

### Inherits From

- MediaDestination

## See Also

### Providing a Destination

object AddMediaMediaDestinationResolutionResult.Success

A media destination that successfully matches an intent.

object MediaDestination

The user’s library or a playlist.

object MediaDestinationLibrary

The user’s library as a destination for an add media intent.

