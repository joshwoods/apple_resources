

- SiriKit Cloud Media
-  PlayMediaControl 

Object

# PlayMediaControl

A configuration for permitted user interactions and other player behaviors during playback.

SiriKit Cloud Media 1.0.2+

``` source
object PlayMediaControl
```

## Properties

`scheme`

PlayMediaControlScheme

 (Required) 

The base set of user controls to make available, and related content behaviors to use.

`commands`

PlayMediaControlCommandSet

A set of commands and their desired availabilities to override the default behavior of the `scheme`.

`activity`

PlayMediaControlActivity

A schedule for the client to report playback progress to the Report Playback Progress and Activity endpoint.

## See Also

### Customizing Playback Controls

object QueueControlMapping

A dictionary of configuration names and the media controls they permit.

type PlayMediaControlScheme

Default playback controls and settings for common content types.

object PlayMediaControlCommandSet

A set of modifications to apply to the default set of available playback controls.

