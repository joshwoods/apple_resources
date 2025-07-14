

- SiriKit Cloud Media
- ExtensionConfig
- ExtensionConfig.Media
- ExtensionConfig.Media.Queues
-  ExtensionConfig.Media.Queues.ContentPlaybackFailure 

Object

# ExtensionConfig.Media.Queues.ContentPlaybackFailure

Configuration details for your service’s content playback failure endpoint.

SiriKit Cloud Media 1.0.2+

``` source
object ExtensionConfig.Media.Queues.ContentPlaybackFailure
```

## Properties

`url`

`string`

 (Required) 

The relative path for the client to access the `contentPlaybackFailure` endpoint. For more information, see contentPlaybackFailure.

Default: `/queues/contentPlaybackFailure`

Minimum length: `1`

Maximum length: `4000`

## See Also

### Requiring Headers and Specifying Paths for Specific Queue Endpoints

object ExtensionConfig.Media.Queues.PlayMedia

Configuration details for your service’s media playback queue.

object ExtensionConfig.Media.Queues.UpdateActivity

Configuration details for your service’s update activity endpoint.

object ExtensionConfig.Media.Queues.ContentProtectionKey

Configuration details for your service’s content protection key endpoint.

