

- AVFoundation
- AVAssetResourceLoadingRequest
-  persistentContentKey(fromKeyVendorResponse:options:) Deprecated

Instance Method

# persistentContentKey(fromKeyVendorResponse:options:)

Obtains a persistable content key from a context.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.15–15.0DeprecatedtvOS 9.0–18.0Deprecated

``` source
func persistentContentKey(
    fromKeyVendorResponse keyVendorResponse: Data,
    options: [String : Any]? = nil
) throws -> Data
```

Deprecated

Use -\[AVPersistableContentKeyRequest persistableContentKeyFromKeyVendorResponse:options:error:\] instead

## Parameters 

`keyVendorResponse`  

The response returned from the key vendor as a result of a request generated from streamingContentKeyRequestData(forApp:contentIdentifier:options:).

`options`  

Additional information necessary to obtain the key, or `nil` if no additional information is required.

## Return Value

The persistable content key.

## Discussion

The data returned from this method may be used to immediately satisfy an AVAssetResourceLoadingDataRequest, as well as any subsequent requests for the same key URL. The value of contentType must be set to AVStreamingKeyDeliveryPersistentContentKeyType when responding with data created with this method.

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

let AVAssetResourceLoadingRequestStreamingContentKeyRequestRequiresPersistentKey: String

Specifies whether the content key request requires a persistable key to be returned from the key vendor.

Deprecated

