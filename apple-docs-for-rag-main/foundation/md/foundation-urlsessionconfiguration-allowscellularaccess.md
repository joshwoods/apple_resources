

- Foundation
- URLSessionConfiguration
-  allowsCellularAccess 

Instance Property

# allowsCellularAccess

A Boolean value that determines whether connections should be made over a cellular network.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var allowsCellularAccess: Bool { get set }
```

## Discussion

This property controls whether tasks in sessions based on this session configuration are allowed to make connections over a cellular network.

The default value is true.

For more information, read Restrict Cellular Networking Correctly.

## See Also

### Setting general properties

var identifier: String?

The background session identifier of the configuration object.

var httpAdditionalHeaders: [AnyHashable : Any]?

A dictionary of additional headers to send with requests.

var networkServiceType: NSURLRequest.NetworkServiceType

The type of network service for all tasks within network sessions to enable Cellular Network Slicing.

var timeoutIntervalForRequest: TimeInterval

The timeout interval to use when waiting for additional data.

var timeoutIntervalForResource: TimeInterval

The maximum amount of time that a resource request should be allowed to take.

var sharedContainerIdentifier: String?

The identifier for the shared container into which files in background URL sessions should be downloaded.

var waitsForConnectivity: Bool

A Boolean value that indicates whether the session should wait for connectivity to become available, or fail immediately.

var usesClassicLoadingMode: Bool

