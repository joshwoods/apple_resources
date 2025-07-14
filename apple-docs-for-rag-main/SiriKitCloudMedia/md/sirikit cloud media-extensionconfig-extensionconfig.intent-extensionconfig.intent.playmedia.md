

- SiriKit Cloud Media
- ExtensionConfig
- ExtensionConfig.Intent
-  ExtensionConfig.Intent.PlayMedia 

Object

# ExtensionConfig.Intent.PlayMedia

Configuration details for your service’s play media intent.

SiriKit Cloud Media 1.0.2+

``` source
object ExtensionConfig.Intent.PlayMedia
```

## Properties

`opt`

`[string]`

Optional intent-handling steps that Process a Play Media Intent supports.

Possible Values: `resolvePlayShuffled, resolvePlaybackRepeatMode, resolvePlaybackQueueLocation, resolveResumePlayback`

## Discussion

To specify that your service only implements the required methods, provide an empty array for the `opt` property. You may omit the `opt` property if your service implements all of the optional methods.

## Relationships

### Inherits From

- ExtensionEndpointConfig

## See Also

### Specifying Required Headers and Supported Processing for Each Intent

object ExtensionConfig.Intent.AddMedia

Configuration details for your service’s add media intent.

object ExtensionConfig.Intent.UpdateMediaAffinity

Configuration details for your service’s update media affinity intent.

