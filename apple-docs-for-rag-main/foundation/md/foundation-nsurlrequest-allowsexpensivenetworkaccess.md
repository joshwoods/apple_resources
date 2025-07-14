

- Foundation
- NSURLRequest
-  allowsExpensiveNetworkAccess 

Instance Property

# allowsExpensiveNetworkAccess

A Boolean value that indicates whether connections may use a network interface that the system considers expensive.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var allowsExpensiveNetworkAccess: Bool { get }
```

## Discussion

The system determines what constitutes “expensive” based on the nature of the network interface and other factors. iOS 13 considers most cellular networks and personal hotspots expensive. If there are no nonexpensive network interfaces available and the request’s allowsExpensiveNetworkAccess property is false, any task created from the request fails. In this case, the error provided when the task fails has a networkUnavailableReason property whose value is NSURLErrorNetworkUnavailableReasonExpensive.

Limit your app’s of use of expensive network access to user-initiated tasks, and put off discretionary tasks until a nonexpensive interface becomes available.

## See Also

### Supporting limited modes

var allowsConstrainedNetworkAccess: Bool

A Boolean value that indicates whether connections may use the network when the user has specified Low Data Mode.

