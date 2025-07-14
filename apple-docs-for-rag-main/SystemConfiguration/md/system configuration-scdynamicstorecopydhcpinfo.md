

- System Configuration
-  SCDynamicStoreCopyDHCPInfo 

Function

# SCDynamicStoreCopyDHCPInfo

Returns the DHCP information for the specified service.

macOS 10.1+

``` source
CFDictionaryRef SCDynamicStoreCopyDHCPInfo(SCDynamicStoreRef store, CFStringRef serviceID);
```

## Parameters 

`store`  

The dynamic store session that should be used for communication with the server. If this is `NULL`, a temporary session is used.

`serviceID`  

The service ID. Pass `NULL` to retrieve information for the primary service.

## Return Value

A dictionary containing DHCP information if successful, or `NULL` if unsuccessful. You must use the CFRelease function to release return values other than `NULL`.

## Discussion

Use DHCPInfoGetOptionData to extract individual options from the dictionary returned by this function.

## See Also

### Group

DHCPInfoGetOptionData

Returns DHCP option data, if present.

DHCPInfoGetLeaseStartTime

Returns the lease start time data.

