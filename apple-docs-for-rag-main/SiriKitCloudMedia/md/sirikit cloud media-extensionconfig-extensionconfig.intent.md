

- SiriKit Cloud Media
- ExtensionConfig
-  ExtensionConfig.Intent 

Object

# ExtensionConfig.Intent

Instructions for accessing your media service’s intent endpoints.

SiriKit Cloud Media 1.0.2+

``` source
object ExtensionConfig.Intent
```

## Properties

`hdr`

ExtensionConfig.Intent.Hdr

Headers to include with requests to intent endpoints.

`addMedia`

ExtensionConfig.Intent.AddMedia

Details specific to Process an Add Media Intent.

`playMedia`

ExtensionConfig.Intent.PlayMedia

 (Required) 

Details specific to Process a Play Media Intent.

`updateMediaAffinity`

ExtensionConfig.Intent.UpdateMediaAffinity

Details specific to updateMediaAffinity.

## Topics

### Requiring Headers for All Intent Requests

object ExtensionConfig.Intent.Hdr

Headers to include with requests to intent endpoints.

### Specifying Required Headers and Supported Processing for Each Intent

object ExtensionConfig.Intent.AddMedia

Configuration details for your service’s add media intent.

object ExtensionConfig.Intent.PlayMedia

Configuration details for your service’s play media intent.

object ExtensionConfig.Intent.UpdateMediaAffinity

Configuration details for your service’s update media affinity intent.

## See Also

### Describing Supported Intent Endpoints

object ExtensionEndpointConfig

Instructions for accessing an intent endpoint.

