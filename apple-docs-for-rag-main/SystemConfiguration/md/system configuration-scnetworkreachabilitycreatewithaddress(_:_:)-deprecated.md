

- System Configuration
-  SCNetworkReachabilityCreateWithAddress(\_:\_:) Deprecated

Function

# SCNetworkReachabilityCreateWithAddress(\_:\_:)

Creates a reachability reference to the specified network address.

iOS 2.0–17.4DeprecatediPadOS 2.0–17.4DeprecatedMac Catalyst 13.1–17.4DeprecatedmacOS 10.3–14.4DeprecatedtvOSDeprecatedvisionOS 1.0–1.1Deprecated

``` source
func SCNetworkReachabilityCreateWithAddress(
    _ allocator: CFAllocator?,
    _ address: UnsafePointer
) -> SCNetworkReachability?
```

## Parameters 

`allocator`  

The allocator to use. Pass `NULL` or kCFAllocatorDefault to use the default allocator.

`address`  

The address of the desired host. The value of this parameter is copied into the new object.

## Return Value

A new immutable reachability reference. You must release the returned value.

## Discussion

You can use the reachability reference returned by this function to monitor the reachability of the target host.

## See Also

### Creating a Reachability Reference

func SCNetworkReachabilityCreateWithAddressPair(CFAllocator?, UnsafePointer&lt;sockaddr>?, UnsafePointer&lt;sockaddr>?) -> SCNetworkReachability?

Creates a reachability reference to the specified network address.

Deprecated

func SCNetworkReachabilityCreateWithName(CFAllocator?, UnsafePointer&lt;CChar>) -> SCNetworkReachability?

Creates a reachability reference to the specified network host or node name.

Deprecated

