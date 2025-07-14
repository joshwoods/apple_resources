

- SiriKit Cloud Media
- ExtensionConfig
- ExtensionConfig.Media
- ExtensionConfig.Media.Queues
-  ExtensionConfig.Media.Queues.UpdateActivity 

Object

# ExtensionConfig.Media.Queues.UpdateActivity

Configuration details for your service’s update activity endpoint.

SiriKit Cloud Media 1.0.2+

``` source
object ExtensionConfig.Media.Queues.UpdateActivity
```

## Properties

`url`

`string`

The relative path for the client to access updateActivity.

Default: `/queues/updateActivity`

Minimum length: `1`

Maximum length: `4000`

`hdr`

ExtensionConfig.Media.Queues.UpdateActivity.Hdr

Headers to include with requests to this endpoint.

## Topics

### Requiring Headers

object ExtensionConfig.Media.Queues.UpdateActivity.Hdr

Headers to include with requests to the update activity endpoint.

## See Also

### Requiring Headers and Specifying Paths for Specific Queue Endpoints

object ExtensionConfig.Media.Queues.PlayMedia

Configuration details for your service’s media playback queue.

object ExtensionConfig.Media.Queues.ContentPlaybackFailure

Configuration details for your service’s content playback failure endpoint.

object ExtensionConfig.Media.Queues.ContentProtectionKey

Configuration details for your service’s content protection key endpoint.

