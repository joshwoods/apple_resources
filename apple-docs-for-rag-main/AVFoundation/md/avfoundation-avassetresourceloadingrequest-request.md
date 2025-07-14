

- AVFoundation
- AVAssetResourceLoadingRequest
-  request 

Instance Property

# request

The URL request object for the resource.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var request: URLRequest { get }
```

## Discussion

Use the value in this property to identify the requested resource and to formulate an appropriate response object.

## See Also

### Accessing the Request Data

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

let AVAssetResourceLoadingRequestStreamingContentKeyRequestRequiresPersistentKey: String

Specifies whether the content key request requires a persistable key to be returned from the key vendor.

Deprecated

