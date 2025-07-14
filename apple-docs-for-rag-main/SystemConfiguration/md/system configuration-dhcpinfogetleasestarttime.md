

- System Configuration
-  DHCPInfoGetLeaseStartTime 

Function

# DHCPInfoGetLeaseStartTime

Returns the lease start time data.

macOS 10.1+

``` source
CFDateRef DHCPInfoGetLeaseStartTime(CFDictionaryRef info);
```

## Parameters 

`info`  

The DHCP information dictionary returned by SCDynamicStoreCopyDHCPInfo. Do not pass in a `NULL` dictionary.

## Return Value

Data that corresponds to the lease start time, if this information is present, or `NULL` if the information is not present or if the configuration method is not DHCP.

## See Also

### Group

SCDynamicStoreCopyDHCPInfo

Returns the DHCP information for the specified service.

DHCPInfoGetOptionData

Returns DHCP option data, if present.

