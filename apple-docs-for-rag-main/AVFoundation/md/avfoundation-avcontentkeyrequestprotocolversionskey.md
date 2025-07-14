

- AVFoundation
-  AVContentKeyRequestProtocolVersionsKey 

Global Variable

# AVContentKeyRequestProtocolVersionsKey

A key that specifies the versions of the content protection protocol supported by the application.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+macOS 10.12.4+tvOS 10.2+visionOS 1.0+watchOS 7.0+

``` source
let AVContentKeyRequestProtocolVersionsKey: String
```

## Discussion

The contents of this key are an NSArray or one or more NSNumber objects.

## See Also

### Getting Content Key Request Data

func makeStreamingContentKeyRequestData(forApp: Data, contentIdentifier: Data?, options: [String : Any]?, completionHandler: (Data?, (any Error)?) -> Void)

Obtains encrypted key request data for a specific combination of app and content.

let AVContentKeyRequestRequiresValidationDataInSecureTokenKey: String

A key that requires the secure token to have extended validation data.

