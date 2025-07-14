

- Foundation
- URLSessionConfiguration
-  waitsForConnectivity 

Instance Property

# waitsForConnectivity

A Boolean value that indicates whether the session should wait for connectivity to become available, or fail immediately.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var waitsForConnectivity: Bool { get set }
```

## Mentioned in 

Fetching website data into memory

## Discussion

Connectivity might be temporarily unavailable for several reasons. For example, a device might only have a cellular connection when allowsCellularAccess is set to `false`, or the device might require a VPN connection but none is available. If the value of this property is `true` and sufficient connectivity is unavailable, the session calls the urlSession(_:taskIsWaitingForConnectivity:) method of URLSessionTaskDelegate and waits for connectivity. When connectivity becomes available, the task begins its work and ultimately calls the delegate or completion handler as usual.

If the value of the property is `false` and connectivity is unavailable, the connection fails immediately with an error, such as NSURLErrorNotConnectedToInternet.

This property is relevant only during the establishment of a connection. If a connection is established and then drops, the completion handler or delegate receives an error, such as NSURLErrorNetworkConnectionLost. For help dealing with dropped connections, see Handling “The network connection was lost” Errors.

This property is ignored by background sessions, which always wait for connectivity.

## See Also

### Setting general properties

var identifier: String?

The background session identifier of the configuration object.

var httpAdditionalHeaders: [AnyHashable : Any]?

A dictionary of additional headers to send with requests.

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

var usesClassicLoadingMode: Bool

