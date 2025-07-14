

- AVFoundation
- AVAssetResourceLoadingRequest
-  requestor 

Instance Property

# requestor

The asset resource requestor that made the request.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
var requestor: AVAssetResourceLoadingRequestor { get }
```

## See Also

### Accessing the Request Data

var request: URLRequest

The URL request object for the resource.

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

let AVAssetResourceLoadingRequestStreamingContentKeyRequestRequiresPersistentKey: String

Specifies whether the content key request requires a persistable key to be returned from the key vendor.

Deprecated

