

- System Configuration
-  DHCPInfoGetOptionData 

Function

# DHCPInfoGetOptionData

Returns DHCP option data, if present.

macOS 10.1+

``` source
CFDataRef DHCPInfoGetOptionData(CFDictionaryRef info, UInt8 code);
```

## Parameters 

`info`  

The DHCP information dictionary returned by SCDynamicStoreCopyDHCPInfo. Do not pass in a `NULL` dictionary.

`code`  

The DHCP option code to get data for. (See RFC 2132 for more information on this code.)

## Return Value

The DHCP option data if present, or `NULL` if the data is not present. You must not release the return value.

## See Also

### Group

SCDynamicStoreCopyDHCPInfo

Returns the DHCP information for the specified service.

DHCPInfoGetLeaseStartTime

Returns the lease start time data.

