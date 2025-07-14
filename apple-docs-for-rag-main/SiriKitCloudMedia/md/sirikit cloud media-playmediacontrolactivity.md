

- SiriKit Cloud Media
-  PlayMediaControlActivity 

Object

# PlayMediaControlActivity

Options for reporting playback progress.

SiriKit Cloud Media 1.0.2+

``` source
object PlayMediaControlActivity
```

## Properties

`playElapsed`

`uint32`

The number of seconds the client plays a piece of content before sending a `local.playing.elapsed` event.

Minimum: `5`

`playElapsedInterval`

`uint32`

The number of seconds the client waits before sending a subsequent `local.playing.elapsed` event.

Minimum: `5`

`playPaused`

`uint32`

The minimum pause duration, in seconds, that the client reports.

Default: `5`

Minimum: `5`

Maximum: `60`

## Discussion

Provide these values in a Queue to configure when the client sends requests to your Report Playback Progress and Activity endpoint.

If you specify both `playElapsedInterval` and `playElapsed`, the client sends the first report after it plays `playElapsed` seconds of content. Then it sends additional reports according to the `playElapsedInterval`, counting from the beginning of the content. For example, if you specify `45` for `playElapsed` and `30` for `playElapsedInterval`, the client sends reports after 45, 60, 90, and 120 seconds of playback.

If you specify `playElapsedInterval`, but not `playElapsed`, the client uses the `playElapsedInterval` for both.

## See Also

### Device Configuration

Configure Your Service Endpoints

Provide configuration details for your media server’s endpoints to a HomePod speaker or an Apple TV.

type ExtensionConfigTag

A unique identifier for a specific media service configuration.

object ExtensionConfig

Instructions for accessing your media service’s endpoints.

