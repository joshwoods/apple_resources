

- SiriKit Cloud Media
-  PlayMediaRequest 

Object

# PlayMediaRequest

A request for a media playback queue.

SiriKit Cloud Media 1.0.2+

``` source
object PlayMediaRequest
```

## Properties

`constraints`

Constraints

 (Required) 

Limitations on the type and quantity of content the client can receive.

`userActivity`

UserActivity

 (Required) 

A description of the playback queue. Your service provides the UserActivity after it successfully handles a play media intent.

`version`

`string`

 (Required) 

The version of the `SiriKitMediaAPI` library the client uses.

Value: `/[0-9]+\.[0-9]+\.[0-9]+/`

