

- SiriKit Cloud Media
- ExtensionConfig
- ExtensionConfig.Media
- ExtensionConfig.Media.Queues
-  ExtensionConfig.Media.Queues.ContentProtectionKey 

Object

# ExtensionConfig.Media.Queues.ContentProtectionKey

Configuration details for your service’s content protection key endpoint.

SiriKit Cloud Media 1.0.2+

``` source
object ExtensionConfig.Media.Queues.ContentProtectionKey
```

## Properties

`cks`

ExtensionConfig.Media.Queues.ContentProtectionKey.Cks

 (Required) 

The configuration details of your service’s content protection system.

`hdr`

ExtensionConfig.Media.Queues.ContentProtectionKey.Hdr

The headers to include with requests to this endpoint.

`url`

`string`

 (Required) 

The relative path for the client to access the `contentProtectionKey` endpoint. For more information, see contentProtectionKey.

Default: `/queues/contentProtectionKey`

Minimum length: `1`

Maximum length: `4000`

## Topics

### Requiring Headers

object ExtensionConfig.Media.Queues.ContentProtectionKey.Cks

Configuration details for your service’s content protection system.

object ExtensionConfig.Media.Queues.ContentProtectionKey.Hdr

Headers to include with requests to the content protection key endpoint.

## See Also

### Requiring Headers and Specifying Paths for Specific Queue Endpoints

object ExtensionConfig.Media.Queues.PlayMedia

Configuration details for your service’s media playback queue.

object ExtensionConfig.Media.Queues.UpdateActivity

Configuration details for your service’s update activity endpoint.

object ExtensionConfig.Media.Queues.ContentPlaybackFailure

Configuration details for your service’s content playback failure endpoint.

