

- AVFoundation
- AVContentKeySessionDelegate
-  contentKeySession(\_:didProvide:) 

Instance Method

# contentKeySession(\_:didProvide:)

Provides the receiver with a new content key request object to process a persistable content key.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+macOS 10.12.4+tvOS 10.2+visionOS 1.0+watchOS 7.0+

``` source
optional func contentKeySession(
    _ session: AVContentKeySession,
    didProvide keyRequest: AVPersistableContentKeyRequest
)
```

## Parameters 

`session`  

The content key session that is providing the new persistable content key request.

`keyRequest`  

The request for a new persistable content key.

## See Also

### Providing New Content Key Requests

func contentKeySession(AVContentKeySession, didProvide: AVContentKeyRequest)

Provides the receiver with a new content key request object.

**Required**

func contentKeySession(AVContentKeySession, didProvideRenewingContentKeyRequest: AVContentKeyRequest)

Provides the receiver with a new content key request object for the renewal of an existing content key.

