

- System Configuration
-  SCNetworkReachabilityCreateWithName(\_:\_:) Deprecated

Function

# SCNetworkReachabilityCreateWithName(\_:\_:)

Creates a reachability reference to the specified network host or node name.

iOS 2.0–17.4DeprecatediPadOS 2.0–17.4DeprecatedMac Catalyst 13.1–17.4DeprecatedmacOS 10.3–14.4DeprecatedtvOSDeprecatedvisionOS 1.0–1.1Deprecated

``` source
func SCNetworkReachabilityCreateWithName(
    _ allocator: CFAllocator?,
    _ nodename: UnsafePointer
) -> SCNetworkReachability?
```

## Parameters 

`allocator`  

The allocator to use. Pass `NULL` or kCFAllocatorDefault to use the default allocator.

`nodename`  

The node name of the desired host. This name is the same as that passed to the gethostbyname or getaddrinfo functions. The value of this parameter is copied into the new object.

## Return Value

A new immutable reachability reference. You must release the returned value.

## Discussion

You can use the reachability reference returned by this function to monitor the reachability of the target host.

## See Also

### Creating a Reachability Reference

func SCNetworkReachabilityCreateWithAddress(CFAllocator?, UnsafePointer&lt;sockaddr>) -> SCNetworkReachability?

Creates a reachability reference to the specified network address.

Deprecated

func SCNetworkReachabilityCreateWithAddressPair(CFAllocator?, UnsafePointer&lt;sockaddr>?, UnsafePointer&lt;sockaddr>?) -> SCNetworkReachability?

Creates a reachability reference to the specified network address.

Deprecated

