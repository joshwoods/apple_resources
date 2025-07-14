

- dnssd
-  DNSServiceGetProperty(\_:\_:\_:) 

Function

# DNSServiceGetProperty(\_:\_:\_:)

Gets the specified property of a service.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func DNSServiceGetProperty(
    _ property: UnsafePointer!,
    _ result: UnsafeMutableRawPointer!,
    _ size: UnsafeMutablePointer!
) -> DNSServiceErrorType
```

## Parameters 

`property`  

The requested property. Currently the only property defined is kDNSServiceProperty_DaemonVersion.

`result`  

Place to store result. For retrieving DaemonVersion, this should be the address of a uint32_t.

`size`  

Pointer to uint32_t containing size of the result location. For retrieving DaemonVersion, this should be sizeof(uint32_t). On return the uint32_t is updated to the size of the data returned. For DaemonVersion, the returned size is always sizeof(uint32_t), but future properties could be defined which return variable-sized results.

## Return Value

Returns kDNSServiceErr_NoError on success, or kDNSServiceErr_ServiceNotRunning if the daemon (or “system service” on Windows) is not running.

## Mentioned in 

\_DNS_SD_H

