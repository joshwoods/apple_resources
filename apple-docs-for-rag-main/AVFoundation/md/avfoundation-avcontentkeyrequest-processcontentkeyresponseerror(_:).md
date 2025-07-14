

- AVFoundation
- AVContentKeyRequest
-  processContentKeyResponseError(\_:) 

Instance Method

# processContentKeyResponseError(\_:)

Tells the receiver that the app was unable to obtain a content key response.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+macOS 10.12.4+tvOS 10.2+visionOS 1.0+watchOS 7.0+

``` source
func processContentKeyResponseError(_ error: any Error)
```

## Parameters 

`error`  

An NSError that describes why the content key response failed.

## See Also

### Responding to the Content Key Request

func respondByRequestingPersistableContentKeyRequest()

Tells the receiver that the app requires a persistable content key request object for processing.

Deprecated

func processContentKeyResponse(AVContentKeyResponse)

Sends the specified content key response to the receiver for processing.

func respondByRequestingPersistableContentKeyRequest()

Tells the receiver that the app requires a persistable content key request object for processing.

Deprecated

