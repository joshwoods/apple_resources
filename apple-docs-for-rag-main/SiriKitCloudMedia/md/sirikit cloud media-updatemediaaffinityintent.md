

- SiriKit Cloud Media
-  UpdateMediaAffinityIntent 

Object

# UpdateMediaAffinityIntent

An object that describes a user’s stated preference regarding media items.

SiriKit Cloud Media 1.0.2+

``` source
object UpdateMediaAffinityIntent
```

## Properties

`class`

`string`

 (Required) 

The specific type of intent.

Value: `UpdateMediaAffinityIntent`

`affinityType`

MediaAffinityType

The user’s preference for the media items.

`mediaItems`

`[`MediaItem`]`

Specific media items the user expresses a preference for.

`mediaSearch`

MediaSearch

The description of the media items the user expresses a preference for.

## Relationships

### Inherits From

- Intent

## See Also

### Processing an Update Media Affinity Intent

object UpdateMediaAffinityIntentHandlingInvocation

A request to process an update media affinity intent.

type UpdateMediaAffinityIntentHandlingInvocationResponse

The service’s response to a request to process an update media affinity intent.

