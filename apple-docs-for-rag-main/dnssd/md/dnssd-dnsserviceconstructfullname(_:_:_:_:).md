

- dnssd
-  DNSServiceConstructFullName(\_:\_:\_:\_:) 

Function

# DNSServiceConstructFullName(\_:\_:\_:\_:)

Concatenates a three-part domain name (as returned by the above callbacks) into a properly-escaped full domain name.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func DNSServiceConstructFullName(
    _ fullName: UnsafeMutablePointer!,
    _ service: UnsafePointer!,
    _ regtype: UnsafePointer!,
    _ domain: UnsafePointer!
) -> DNSServiceErrorType
```

## Parameters 

`fullName`  

A pointer to a buffer that where the resulting full domain name is to be written. The buffer must be kDNSServiceMaxDomainName (1009) bytes in length to accommodate the longest legal domain name without buffer overrun.

`service`  

The service name - any dots or backslashes must NOT be escaped. May be NULL (to construct a PTR record name, e.g. “\_ftp.\_tcp.apple.com.”).

`regtype`  

The service type followed by the protocol, separated by a dot (e.g. “\_ftp.\_tcp”).

`domain`  

The domain name, e.g. “apple.com.”. Literal dots or backslashes, if any, must be escaped, e.g. “1st. Floor.apple.com.”

## Return Value

Returns kDNSServiceErr_NoError (0) on success, kDNSServiceErr_BadParam on error.

## Discussion

Note that callbacks in the above functions ALREADY ESCAPE strings where necessary.

