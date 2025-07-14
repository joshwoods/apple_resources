

- Foundation
- URLSessionConfiguration
-  allowsExpensiveNetworkAccess 

Instance Property

# allowsExpensiveNetworkAccess

A Boolean value that indicates whether connections may use a network interface that the system considers expensive.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var allowsExpensiveNetworkAccess: Bool { get set }
```

## Discussion

The system determines what constitutes “expensive” based on the nature of the network interface and other factors. iOS 13 considers most cellular networks and personal hotspots expensive. If there are no nonexpensive network interfaces available and the session’s allowsExpensiveNetworkAccess property is false, any task created from the session fails. In this case, the error provided when the task fails has a networkUnavailableReason property whose value is NSURLErrorNetworkUnavailableReasonExpensive.

You can limit your app’s of use of expensive network access to user-initiated tasks, and put off discretionary tasks until a nonexpensive interface becomes available. To do this, set allowsExpensiveNetworkAccess (and allowsConstrainedNetworkAccess) to false and waitsForConnectivity to true. This way, your URLSessionTask waits for a suitable interface to become available before sending or receiving data.

To test the behavior of this property, you can override the device’s current values for cellular and Wi-Fi cost in Settings \> Developer \> Network Override.

Tip

Prefer basing your app’s policy logic around the allowsConstrainedNetworkAccess property rather than this one. People using your app can use the “Low Data Mode” setting to set the constrained status, and thereby choose to use a potentially expensive network.

## See Also

### Supporting limited modes

var allowsConstrainedNetworkAccess: Bool

A Boolean value that indicates whether connections may use the network when the user has specified Low Data Mode.

