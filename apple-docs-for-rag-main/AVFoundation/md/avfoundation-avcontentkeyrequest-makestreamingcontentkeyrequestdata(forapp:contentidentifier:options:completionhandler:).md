

- AVFoundation
- AVContentKeyRequest
-  makeStreamingContentKeyRequestData(forApp:contentIdentifier:options:completionHandler:) 

Instance Method

# makeStreamingContentKeyRequestData(forApp:contentIdentifier:options:completionHandler:)

Obtains encrypted key request data for a specific combination of app and content.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+macOS 10.12.4+tvOS 10.2+visionOS 1.0+watchOS 7.0+

``` source
func makeStreamingContentKeyRequestData(
    forApp appIdentifier: Data,
    contentIdentifier: Data?,
    options: [String : Any]? = nil,
    completionHandler handler: @escaping (Data?, (any Error)?) -> Void
)
```

``` source
func makeStreamingContentKeyRequestData(
    forApp appIdentifier: Data,
    contentIdentifier: Data?,
    options: [String : Any]? = nil
) async throws -> Data
```

## Parameters 

`appIdentifier`  

An opaque identifier for the app.

`contentIdentifier`  

An opaque identifier for the content.

`options`  

A dictionary containing any additional information required to obtain the key. The value of this parameter is `nil` when no additional information is required.

`handler`  

A block called after the streaming content key request has been prepared.

contentKeyRequestData  
The streaming content key request data.

error  
An object that describes the error, if one occurred; otherwise, the value is `nil`.

## Discussion

If AVContentKeyRequestProtocolVersionsKey is not specified in the `options` parameter, the default protocol of `1` is used.

## See Also

### Getting Content Key Request Data

let AVContentKeyRequestProtocolVersionsKey: String

A key that specifies the versions of the content protection protocol supported by the application.

let AVContentKeyRequestRequiresValidationDataInSecureTokenKey: String

A key that requires the secure token to have extended validation data.

