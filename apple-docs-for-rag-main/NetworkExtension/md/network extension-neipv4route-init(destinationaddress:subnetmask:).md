

- Network Extension
- NEIPv4Route
-  init(destinationAddress:subnetMask:) 

Initializer

# init(destinationAddress:subnetMask:)

Initialize the NEIPv4Route object.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
init(
    destinationAddress address: String,
    subnetMask: String
)
```

## Parameters 

`address`  

An IPv4 address string. This string is combined with `subnetMask` to specify the destination network of the route.

`subnetMask`  

An IPv4 network mask string. This string is combined with `address` to specify the destination network of the route.

## See Also

### Creating an IPv4 Route

class func `default`() -> NEIPv4Route

A convenience method for creating the default IPv4 route.

