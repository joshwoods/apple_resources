

- SiriKit Cloud Media
-  ExtensionConfig 

Object

# ExtensionConfig

Instructions for accessing your media service’s endpoints.

SiriKit Cloud Media 1.0.2+

``` source
object ExtensionConfig
```

## Properties

`version`

`string`

 (Required) 

The version of this API your service supports.

Value: `/([0-9]+[.]){2}[0-9]+/`

`url`

`string`

The fully qualified base URL for the endpoints your service supports.

Minimum length: `1`

Maximum length: `2000`

`hdr`

ExtensionConfig.Hdr

A dictionary of header names and values for the client to include in requests to any intent endpoint.

`intent`

ExtensionConfig.Intent

 (Required) 

The intent endpoints your service supports.

`media`

ExtensionConfig.Media

 (Required) 

The media endpoints your service supports.

## Topics

### Specifying Request Headers

object ExtensionConfig.Hdr

Headers to include with all requests to the media service.

object ExtensionEndpointConfig.Hdr

Headers to include with requests to intent endpoints.

object ExtensionConfig.Intent.Hdr

Headers to include with requests to intent endpoints.

object ExtensionConfig.Media.Queues.Hdr

Headers to include with requests to media endpoints.

object ExtensionConfig.Media.Queues.PlayMedia.Hdr

Headers to include with requests to media endpoints.

object ExtensionConfig.Media.Queues.UpdateActivity.Hdr

Headers to include with requests to the update activity endpoint.

### Describing Supported Intent Endpoints

object ExtensionEndpointConfig

Instructions for accessing an intent endpoint.

object ExtensionConfig.Intent

Instructions for accessing your media service’s intent endpoints.

### Describing Supported Media Endpoints

object ExtensionConfig.Media

Instructions for accessing your service’s media endpoints.

## See Also

### Device Configuration

Configure Your Service Endpoints

Provide configuration details for your media server’s endpoints to a HomePod speaker or an Apple TV.

type ExtensionConfigTag

A unique identifier for a specific media service configuration.

object PlayMediaControlActivity

Options for reporting playback progress.

