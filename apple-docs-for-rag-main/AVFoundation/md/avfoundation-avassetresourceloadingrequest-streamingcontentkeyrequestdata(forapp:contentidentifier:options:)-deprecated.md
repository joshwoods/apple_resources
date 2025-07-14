

- AVFoundation
- AVAssetResourceLoadingRequest
-  streamingContentKeyRequestData(forApp:contentIdentifier:options:) Deprecated

Instance Method

# streamingContentKeyRequestData(forApp:contentIdentifier:options:)

Obtains key request data for a specific combination of application and content.

iOS 7.0–18.0DeprecatediPadOS 7.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.9–15.0DeprecatedtvOS 9.0–18.0Deprecated

``` source
func streamingContentKeyRequestData(
    forApp appIdentifier: Data,
    contentIdentifier: Data,
    options: [String : Any]? = nil
) throws -> Data
```

Deprecated

Use -\[AVContentKeyRequest makeStreamingContentKeyRequestDataForApp:contentIdentifier:options:completionHandler:\] instead

## Parameters 

`appIdentifier`  

An opaque content identifier for the application. The value of this identifier depends on the particular system used to provide the decryption key.

`contentIdentifier`  

An opaque identifier for the content. The value of this identifier depends on the particular system used to provide the decryption key.

`options`  

Additional information necessary to obtain the key, or `nil` if no additional information is required.

## Return Value

The key request data that must be transmitted to the key vendor to obtain the content key.

## Topics

### Configuration Options

let AVAssetResourceLoadingRequestStreamingContentKeyRequestRequiresPersistentKey: String

Specifies whether the content key request requires a persistable key to be returned from the key vendor.

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

func persistentContentKey(fromKeyVendorResponse: Data, options: [String : Any]?) throws -> Data

Obtains a persistable content key from a context.

Deprecated

let AVAssetResourceLoadingRequestStreamingContentKeyRequestRequiresPersistentKey: String

Specifies whether the content key request requires a persistable key to be returned from the key vendor.

Deprecated

