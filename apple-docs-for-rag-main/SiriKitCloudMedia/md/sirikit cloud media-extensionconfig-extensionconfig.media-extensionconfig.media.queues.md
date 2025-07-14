

- SiriKit Cloud Media
- ExtensionConfig
- ExtensionConfig.Media
-  ExtensionConfig.Media.Queues 

Object

# ExtensionConfig.Media.Queues

Configuration details for your service’s media queue.

SiriKit Cloud Media 1.0.2+

``` source
object ExtensionConfig.Media.Queues
```

## Properties

`hdr`

ExtensionConfig.Media.Queues.Hdr

Headers to include with requests to queue endpoints.

`playMedia`

ExtensionConfig.Media.Queues.PlayMedia

Details specific to your media playback queue.

`updateActivity`

ExtensionConfig.Media.Queues.UpdateActivity

Details specific to your update activity endpoint.

`contentPlaybackFailure`

ExtensionConfig.Media.Queues.ContentPlaybackFailure

Details specific to your content playback failure endpoint.

`contentProtectionKey`

ExtensionConfig.Media.Queues.ContentProtectionKey

Details specific to your content protection key endpoint.

## Topics

### Requiring Headers for all Queue Requests

object ExtensionConfig.Media.Queues.Hdr

Headers to include with requests to media endpoints.

### Requiring Headers and Specifying Paths for Specific Queue Endpoints

object ExtensionConfig.Media.Queues.PlayMedia

Configuration details for your service’s media playback queue.

object ExtensionConfig.Media.Queues.UpdateActivity

Configuration details for your service’s update activity endpoint.

object ExtensionConfig.Media.Queues.ContentPlaybackFailure

Configuration details for your service’s content playback failure endpoint.

object ExtensionConfig.Media.Queues.ContentProtectionKey

Configuration details for your service’s content protection key endpoint.

