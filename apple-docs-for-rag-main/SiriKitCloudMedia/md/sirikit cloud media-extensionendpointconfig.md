

- SiriKit Cloud Media
-  ExtensionEndpointConfig 

Object

# ExtensionEndpointConfig

Instructions for accessing an intent endpoint.

SiriKit Cloud Media 1.0.2+

``` source
object ExtensionEndpointConfig
```

## Properties

`hdr`

ExtensionEndpointConfig.Hdr

Headers the client must include in requests to this endpoint.

`url`

`string`

The path to access this endpoint. The path may be an absolute URL, or relative to the resolved Configure Your Service Endpoints URL. Provide an empty string if your service doesn’t support this endpoint.

Minimum length: `0`

Maximum length: `2000`

## Topics

### Requiring Headers for All Endpoints

object ExtensionEndpointConfig.Hdr

Headers to include with requests to intent endpoints.

## Relationships

### Inherited By

- ExtensionConfig.Intent.AddMedia
- ExtensionConfig.Intent.PlayMedia
- ExtensionConfig.Intent.UpdateMediaAffinity

## See Also

### Describing Supported Intent Endpoints

object ExtensionConfig.Intent

Instructions for accessing your media service’s intent endpoints.

