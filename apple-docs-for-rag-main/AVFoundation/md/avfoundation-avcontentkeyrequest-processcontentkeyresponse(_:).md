

- AVFoundation
- AVContentKeyRequest
-  processContentKeyResponse(\_:) 

Instance Method

# processContentKeyResponse(\_:)

Sends the specified content key response to the receiver for processing.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+macOS 10.12.4+tvOS 10.2+visionOS 1.0+watchOS 7.0+

``` source
func processContentKeyResponse(_ keyResponse: AVContentKeyResponse)
```

## Parameters 

`keyResponse`  

An AVContentKeyResponse object carrying a response to a content key request.

## Discussion

After receiving a content key request and calling makeStreamingContentKeyRequestData(forApp:contentIdentifier:options:completionHandler:) on that request, you must obtain a response to the request in accordance with the protocol used by the entity that controls the use of the media data. Use this method to provide the content key response, to make protected content available for processing.

## See Also

### Responding to the Content Key Request

func respondByRequestingPersistableContentKeyRequest()

Tells the receiver that the app requires a persistable content key request object for processing.

Deprecated

func processContentKeyResponseError(any Error)

Tells the receiver that the app was unable to obtain a content key response.

func respondByRequestingPersistableContentKeyRequest()

Tells the receiver that the app requires a persistable content key request object for processing.

Deprecated

