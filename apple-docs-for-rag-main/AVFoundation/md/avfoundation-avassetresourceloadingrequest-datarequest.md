

- AVFoundation
- AVAssetResourceLoadingRequest
-  dataRequest 

Instance Property

# dataRequest

The range of requested resource data.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var dataRequest: AVAssetResourceLoadingDataRequest? { get }
```

## Discussion

An instance of AVAssetResourceLoadingDataRequest that indicates the range of resource data that’s being requested. The value of this property is `nil` if no data is being requested.

## See Also

### Accessing the Request Data

var request: URLRequest

The URL request object for the resource.

var requestor: AVAssetResourceLoadingRequestor

The asset resource requestor that made the request.

var contentInformationRequest: AVAssetResourceLoadingContentInformationRequest?

The information for a requested resource.

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

