

- SiriKit Cloud Media
-  ContentFailure 

Object

# ContentFailure

An object that describes why the client can’t play a specific piece of content.

SiriKit Cloud Media 1.0.2+

``` source
object ContentFailure
```

## Properties

`errorCode`

`int64`

 (Required) 

The error’s identity.

`errorDomain`

`string`

 (Required) 

The error’s domain. This is `com.apple.sirikitcloudmedia.errorDomain`.

Minimum length: `0`

Maximum length: `500`

`url`

`string`

 (Required) 

The URL of the content the client can’t play.

Minimum length: `0`

Maximum length: `2000`

`underlyingError`

UnderlyingError

An object that, when present, provides additional information about why the content fails to play.

## Discussion

The value of `errorCode` is one of the following:

| Code | Description |
|----|----|
| `0` | The client encountered an unexpected error. |
| `1000` | The number of items in the queue segment exceeds the configured maximum. For more information, see Constraints. |
| `1001` | The client failed to play the specified item. For more information, see UnderlyingError. |
| `1002` | The client failed to obtain a content key for a protected item. |

If you receive a ContentFailure with an `errorCode` of `1002`, check the following:

- The configuration for your service’s certificate URL is correct. For more information, see ExtensionConfig.Media.Queues.ContentProtectionKey.Cks.

- The protected item has a valid `assetIdentifier`.

- Your service’s key server module (KSM) provides a valid content key context (CKC) for the protected item’s `assetIdentifier`. For more information, see FairPlay Streaming Overview.

Note

The client doesn’t send an error if your service provides an invalid content key for the specified `assetIdentifier`.

## See Also

### Playback Failure

Recover from Content Playback Failure

Provide a recovery queue that allows the client to resume playback after an error.

object ContentPlaybackFailureRequest

A request the client sends to recover from failed content playback.

object ContentPlaybackFailureResponse

A response that allows the client to recover from failed content playback.

