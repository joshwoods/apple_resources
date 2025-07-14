

- SiriKit Cloud Media
-  UpdateActivityRequest 

Object

# UpdateActivityRequest

A report of the client’s current playback state and recent user interaction, and an opportunity for your service to modify the client’s playback queue.

SiriKit Cloud Media 1.0.2+

``` source
object UpdateActivityRequest
```

## Properties

`constraints`

Constraints

Limitations on the type and quantity of content to provide in a Queue.

`nowPlaying`

PlayerContext

The content the client is playing.

`previouslyPlaying`

PlayerContext

The content the client plays before the current content.

`report`

QueueActivityReportEvent

 (Required) 

The most-recent control the user interacts with, or the natural transition that occurs most recently.

`timestamp`

`date-time`

 (Required) 

The date and time of the reported event.

`userActivity`

UserActivity

 (Required) 

A description of the playback queue the client is playing.

`version`

`string`

 (Required) 

The version of the `SiriKitMediaAPI` library the client uses.

Value: `/[0-9]+\.[0-9]+\.[0-9]+/`

`contentFailure`

ContentFailure

## See Also

### Playback Events

type QueueActivityReportEvent

An event that occurs during content playback.

Report Playback Progress and Activity

Monitor progress through the playback queue.

object UpdateActivityResponse

Updates to the client’s queue and user activity in response to a report of playback progress.

Process an Update Media Affinity Intent

Record the user’s preference for a specific media item or a broader category of media.

