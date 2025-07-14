

- SiriKit Cloud Media
-  MediaDestinationLibrary 

Object

# MediaDestinationLibrary

The user’s library as a destination for an add media intent.

SiriKit Cloud Media 1.0.2+

``` source
object MediaDestinationLibrary
```

## Properties

`mediaDestinationType`

`string`

 (Required) 

The type of collection the user wants to store their media items in.

Value: `library`

## Relationships

### Inherits From

- MediaDestination

## See Also

### Providing a Destination

object AddMediaMediaDestinationResolutionResult.Success

A media destination that successfully matches an intent.

object MediaDestination

The user’s library or a playlist.

object MediaDestinationPlaylist

A playlist as a destination for an add media intent.

