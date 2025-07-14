

- SiriKit Cloud Media
-  ContentProtectionKeyResponse 

Object

# ContentProtectionKeyResponse

A response to a request for an item’s content protection key.

SiriKit Cloud Media 1.0.2+

``` source
object ContentProtectionKeyResponse
```

## Properties

`keyResponse`

`byte`

An encrypted key response that contains the item’s content key. For FairPlay Streaming, this is the content key context (CKC); for more information, see FairPlay Streaming Overview.

`keySystem`

ContentProtectionKeySystem

The content’s encryption type, which matches the configuration in ExtensionConfig.Media.Queues.ContentProtectionKey.Cks.

`leaseRenewalDeadline`

`double`

The length of time, in seconds, before the content key expires. If your service doesn’t impose time limits, return `0`.

`version`

`string`

The version of the client’s `SiriKitMediaAPI` library.

Maximum length: `25`

Value: `/[0-9]+\.[0-9]+\.[0-9]+/`

## See Also

### Content Protection

Retrieve an Asset’s Content Protection Key

Provide the content key for a specific protected asset.

object ContentProtectionKeyRequest

A request for an item’s content protection key.

type ContentProtectionKeySystem

The content protection key systems that SiriKit Cloud Media supports.

