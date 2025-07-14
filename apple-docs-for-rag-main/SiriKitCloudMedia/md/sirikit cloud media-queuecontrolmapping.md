

- SiriKit Cloud Media
-  QueueControlMapping 

Object

# QueueControlMapping

A dictionary of configuration names and the media controls they permit.

SiriKit Cloud Media 1.0.2+

``` source
object QueueControlMapping
```

## Properties

`default`

PlayMediaControl

 (Required) 

The default playback control configuration to use for content that doesn’t specify a different control scheme.

`Any Key`

PlayMediaControl

A playback control configuration with a name you define that Content objects can refer to.

## See Also

### Customizing Playback Controls

object PlayMediaControl

A configuration for permitted user interactions and other player behaviors during playback.

type PlayMediaControlScheme

Default playback controls and settings for common content types.

object PlayMediaControlCommandSet

A set of modifications to apply to the default set of available playback controls.

