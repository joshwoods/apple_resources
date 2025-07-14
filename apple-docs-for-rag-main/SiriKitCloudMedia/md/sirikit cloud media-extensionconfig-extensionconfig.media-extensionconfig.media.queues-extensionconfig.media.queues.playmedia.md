

- SiriKit Cloud Media
- ExtensionConfig
- ExtensionConfig.Media
- ExtensionConfig.Media.Queues
-  ExtensionConfig.Media.Queues.PlayMedia 

Object

# ExtensionConfig.Media.Queues.PlayMedia

Configuration details for your service’s media playback queue.

SiriKit Cloud Media 1.0.2+

``` source
object ExtensionConfig.Media.Queues.PlayMedia
```

## Properties

`url`

`string`

The relative path for the client to access Get a Media Queue.

Default: `/queues/playMedia`

Minimum length: `1`

Maximum length: `4000`

`hdr`

ExtensionConfig.Media.Queues.PlayMedia.Hdr

Headers to include with requests to this endpoint.

## Topics

### Requiring Headers

object ExtensionConfig.Media.Queues.PlayMedia.Hdr

Headers to include with requests to media endpoints.

## See Also

### Requiring Headers and Specifying Paths for Specific Queue Endpoints

object ExtensionConfig.Media.Queues.UpdateActivity

Configuration details for your service’s update activity endpoint.

object ExtensionConfig.Media.Queues.ContentPlaybackFailure

Configuration details for your service’s content playback failure endpoint.

object ExtensionConfig.Media.Queues.ContentProtectionKey

Configuration details for your service’s content protection key endpoint.

