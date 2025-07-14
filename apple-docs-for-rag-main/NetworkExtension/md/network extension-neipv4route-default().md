

- Network Extension
- NEIPv4Route
-  default() 

Type Method

# default()

A convenience method for creating the default IPv4 route.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
class func `default`() -> NEIPv4Route
```

## Return Value

An NEIPv4Route object containing the default IPv4 route.

## Discussion

Set this route in the `includedRoutes` array in the NEIPv4Settings object to specify that all IPv4 network traffic be routed to the TUN interface by default.

## See Also

### Creating an IPv4 Route

init(destinationAddress: String, subnetMask: String)

Initialize the NEIPv4Route object.

