

- Foundation
- URLSessionConfiguration
-  identifier 

Instance Property

# identifier

The background session identifier of the configuration object.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var identifier: String? { get }
```

## Discussion

The value of this property is set only when you use the background(withIdentifier:) method to create the configuration object. The string uniquely identifies a background session object. In iOS, you use this string in cases where the app was terminated while transfers were occurring in the background. When the app relaunches, it uses the string to recreate the configuration and session objects associated with the transfers.

## See Also

### Setting general properties

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

var waitsForConnectivity: Bool

A Boolean value that indicates whether the session should wait for connectivity to become available, or fail immediately.

var usesClassicLoadingMode: Bool

