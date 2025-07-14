

- SiriKit Cloud Media
-  ContentProtectionKeyRequest 

Object

# ContentProtectionKeyRequest

A request for an item’s content protection key.

SiriKit Cloud Media 1.0.2+

``` source
object ContentProtectionKeyRequest
```

## Properties

`assetIdentifier`

`string`

The item’s content key asset identifier.

Maximum length: `4000`

`context`

PlayerContext

 (Required) 

The content the client is playing.

`keyRequest`

`byte`

 (Required) 

An encrypted key request that contains session, authentication, and integrity information. For FairPlay Streaming, this is the server playback context (SPC); for more information, see FairPlay Streaming Overview.

`keySystem`

ContentProtectionKeySystem

 (Required) 

The content’s encryption type, which must match the configuration in ExtensionConfig.Media.Queues.ContentProtectionKey.Cks.

`userActivity`

UserActivity

 (Required) 

A description of the client’s current playback queue.

`version`

`string`

 (Required) 

The version of the client’s `SiriKitMediaAPI` library.

Maximum length: `25`

Value: `/[0-9]+\.[0-9]+\.[0-9]+/`

## Discussion

If your service implements content protection, the client requests an item’s content protection key after each of the following events:

- The client receives the queue’s initial item.

- The client preloads each subsequent item in the queue.

- The user manually transitions to an item in the queue.

For more information on providing your service’s content protection configuration, see ExtensionConfig.Media.Queues.ContentProtectionKey and Retrieve an Asset’s Content Protection Key.

## See Also

### Content Protection

Retrieve an Asset’s Content Protection Key

Provide the content key for a specific protected asset.

object ContentProtectionKeyResponse

A response to a request for an item’s content protection key.

type ContentProtectionKeySystem

The content protection key systems that SiriKit Cloud Media supports.

