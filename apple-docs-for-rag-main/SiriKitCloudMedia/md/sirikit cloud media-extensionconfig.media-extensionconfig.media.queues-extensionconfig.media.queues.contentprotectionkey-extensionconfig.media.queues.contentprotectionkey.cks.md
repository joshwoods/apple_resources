

- SiriKit Cloud Media
- ExtensionConfig
- 
  - ExtensionConfig
- ExtensionConfig.Media
- ExtensionConfig.Media.Queues
- ExtensionConfig.Media.Queues.ContentProtectionKey
-  ExtensionConfig.Media.Queues.ContentProtectionKey.Cks 

Object

# ExtensionConfig.Media.Queues.ContentProtectionKey.Cks

Configuration details for your service’s content protection system.

SiriKit Cloud Media 1.0.2+

``` source
object ExtensionConfig.Media.Queues.ContentProtectionKey.Cks
```

## Properties

`certUrl`

`string`

The URL of the certicate the client must use to sign requests to the `contentProtectionKey` endpoint. For more information, see contentProtectionKey.

Maximum length: `4000`

`keySystem`

ContentProtectionKeySystem

 (Required) 

The content’s encryption type. The only supported value is `ContentKeySystemFairPlayStreaming`.

## See Also

### Requiring Headers

object ExtensionConfig.Media.Queues.ContentProtectionKey.Hdr

Headers to include with requests to the content protection key endpoint.

