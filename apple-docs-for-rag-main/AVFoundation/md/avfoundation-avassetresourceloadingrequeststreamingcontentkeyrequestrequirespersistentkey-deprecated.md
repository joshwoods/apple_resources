

- AVFoundation
-  AVAssetResourceLoadingRequestStreamingContentKeyRequestRequiresPersistentKey Deprecated

Global Variable

# AVAssetResourceLoadingRequestStreamingContentKeyRequestRequiresPersistentKey

Specifies whether the content key request requires a persistable key to be returned from the key vendor.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.14–15.0DeprecatedtvOS 9.0–18.0Deprecated

``` source
let AVAssetResourceLoadingRequestStreamingContentKeyRequestRequiresPersistentKey: String
```

Deprecated

Use -\[AVPersistableContentKeyRequest persistableContentKeyFromKeyVendorResponse:options:error:\] instead

## See Also

### Accessing the Request Data

var request: URLRequest

The URL request object for the resource.

var requestor: AVAssetResourceLoadingRequestor

The asset resource requestor that made the request.

var contentInformationRequest: AVAssetResourceLoadingContentInformationRequest?

The information for a requested resource.

var dataRequest: AVAssetResourceLoadingDataRequest?

The range of requested resource data.

var redirect: URLRequest?

An URL request instance if the loading request was redirected.

func streamingContentKeyRequestData(forApp: Data, contentIdentifier: Data, options: [String : Any]?) throws -> Data

Obtains key request data for a specific combination of application and content.

Deprecated

func persistentContentKey(fromKeyVendorResponse: Data, options: [String : Any]?) throws -> Data

Obtains a persistable content key from a context.

Deprecated

