

- AVFoundation
- AVContentKeyRequest
-  respondByRequestingPersistableContentKeyRequestAndReturnError() 

Instance Method

# respondByRequestingPersistableContentKeyRequestAndReturnError()

Tells the receiver that the app requires a persistable content key request object for processing.

iOS 11.2+iPadOS 11.2+Mac Catalyst 13.1+macOS 10.15+tvOS 17.0+visionOS 1.0+watchOS 7.0+

**iOS, iPadOS, Mac Catalyst**

``` source
func respondByRequestingPersistableContentKeyRequestAndReturnError() throws
```

**macOS, tvOS, visionOS, watchOS**

``` source
func respondByRequestingPersistableContentKeyRequest() throws
```

## Discussion

To create a key that persists across multiple playback sessions, use this method to request an AVPersistableContentKeyRequest object. If the underlying protocol supports persistable content keys, the delegate receives a persistable content key request via the contentKeySession(_:didProvide:) method. An internalInconsistencyException is returned if your delegate does not respond to contentKeySession(_:didProvide:).

