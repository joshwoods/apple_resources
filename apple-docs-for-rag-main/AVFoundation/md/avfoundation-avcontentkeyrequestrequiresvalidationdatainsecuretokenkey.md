

- AVFoundation
-  AVContentKeyRequestRequiresValidationDataInSecureTokenKey 

Global Variable

# AVContentKeyRequestRequiresValidationDataInSecureTokenKey

A key that requires the secure token to have extended validation data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let AVContentKeyRequestRequiresValidationDataInSecureTokenKey: String
```

## Discussion

You create the value for this key by using persistableContentKey(fromKeyVendorResponse:options:).

## See Also

### Getting Content Key Request Data

func makeStreamingContentKeyRequestData(forApp: Data, contentIdentifier: Data?, options: [String : Any]?, completionHandler: (Data?, (any Error)?) -> Void)

Obtains encrypted key request data for a specific combination of app and content.

let AVContentKeyRequestProtocolVersionsKey: String

A key that specifies the versions of the content protection protocol supported by the application.

