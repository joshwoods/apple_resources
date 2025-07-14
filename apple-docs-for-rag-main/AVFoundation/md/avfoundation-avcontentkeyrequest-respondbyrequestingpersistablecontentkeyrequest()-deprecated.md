

- AVFoundation
- AVContentKeyRequest
-  respondByRequestingPersistableContentKeyRequest() Deprecated

Instance Method

# respondByRequestingPersistableContentKeyRequest()

Tells the receiver that the app requires a persistable content key request object for processing.

iOS 10.3–11.2DeprecatediPadOS 10.3–11.2DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func respondByRequestingPersistableContentKeyRequest()
```

Deprecated

Use respondByRequestingPersistableContentKeyRequestAndReturnError().

## Discussion

To create a key that persists across multiple playback sessions, use this method to request an AVPersistableContentKeyRequest object. If the underlying protocol supports persistable content keys, the delegate receives a persistable content key request via the contentKeySession(_:didProvide:) method. An internalInconsistencyException is returned if your delegate does not respond to contentKeySession(_:didProvide:).

## See Also

### Responding to the Content Key Request

func processContentKeyResponse(AVContentKeyResponse)

Sends the specified content key response to the receiver for processing.

func processContentKeyResponseError(any Error)

Tells the receiver that the app was unable to obtain a content key response.

