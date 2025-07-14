

- SiriKit Cloud Media
-  AddMediaIntent 

Object

# AddMediaIntent

An object that describes the user’s request to add media items to their library or to a specific playlist.

SiriKit Cloud Media 1.0.2+

``` source
object AddMediaIntent
```

## Properties

`class`

`string`

 (Required) 

The specific type of intent.

Value: `AddMediaIntent`

`mediaItems`

`[`MediaItem`]`

The media items to add to the user’s library or to a playlist.

`mediaSearch`

MediaSearch

Parameters that describe the media items to add to the user’s library or to a playlist.

`mediaDestination`

MediaDestination

The library or playlist to modify.

## Relationships

### Inherits From

- Intent

## See Also

### Processing an Add Media Intent

object AddMediaIntentHandlingInvocation

A request to process an add media intent.

type AddMediaIntentHandlingInvocationResponse

The service’s response to a request to process an add media intent.

