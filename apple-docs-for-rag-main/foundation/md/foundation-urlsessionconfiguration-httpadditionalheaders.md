

- Foundation
- URLSessionConfiguration
-  httpAdditionalHeaders 

Instance Property

# httpAdditionalHeaders

A dictionary of additional headers to send with requests.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var httpAdditionalHeaders: [AnyHashable : Any]? { get set }
```

## Discussion

This property specifies additional headers that are added to all tasks within sessions based on this configuration. For example, you might set the `User-Agent` header so that it is automatically included in every request your app makes through sessions based on this configuration.

An URLSession object is designed to handle various aspects of the HTTP protocol for you. As a result, you should not modify the following headers:

- `Authorization`

- `Connection`

- `Host`

- `Proxy-Authenticate`

- `Proxy-Authorization`

- `WWW-Authenticate`

Additionally, if the length of your upload body data can be determined automatically—for example, if you provide the body content with an NSData object—the value of `Content-Length` is set for you.

If the same header appears in both this array and the request object (where applicable), the request object’s value takes precedence.

The default value is an empty array.

## See Also

### Setting general properties

var identifier: String?

The background session identifier of the configuration object.

var networkServiceType: NSURLRequest.NetworkServiceType

The type of network service for all tasks within network sessions to enable Cellular Network Slicing.

var allowsCellularAccess: Bool

A Boolean value that determines whether connections should be made over a cellular network.

var timeoutIntervalForRequest: TimeInterval

The timeout interval to use when waiting for additional data.

var timeoutIntervalForResource: TimeInterval

The maximum amount of time that a resource request should be allowed to take.

var sharedContainerIdentifier: String?

The identifier for the shared container into which files in background URL sessions should be downloaded.

var waitsForConnectivity: Bool

A Boolean value that indicates whether the session should wait for connectivity to become available, or fail immediately.

var usesClassicLoadingMode: Bool

