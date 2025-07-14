

- SiriKit Cloud Media
-  UpdateActivityResponse 

Object

# UpdateActivityResponse

Updates to the client’s queue and user activity in response to a report of playback progress.

SiriKit Cloud Media 1.0.2+

``` source
object UpdateActivityResponse
```

## Properties

`queue`

Queue

A sequence of playback content to replace or modify the client’s current playback queue.

`userActivity`

UserActivity

A new user activity for the client to use in future requests to queue endpoints.

## See Also

### Playback Events

type QueueActivityReportEvent

An event that occurs during content playback.

Report Playback Progress and Activity

Monitor progress through the playback queue.

object UpdateActivityRequest

A report of the client’s current playback state and recent user interaction, and an opportunity for your service to modify the client’s playback queue.

Process an Update Media Affinity Intent

Record the user’s preference for a specific media item or a broader category of media.

