

- dnssd
-  DNSServiceBrowse(\_:\_:\_:\_:\_:\_:\_:) 

Function

# DNSServiceBrowse(\_:\_:\_:\_:\_:\_:\_:)

Browses for available services.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func DNSServiceBrowse(
    _ sdRef: UnsafeMutablePointer!,
    _ flags: DNSServiceFlags,
    _ interfaceIndex: UInt32,
    _ regtype: UnsafePointer!,
    _ domain: UnsafePointer!,
    _ callBack: DNSServiceBrowseReply!,
    _ context: UnsafeMutableRawPointer!
) -> DNSServiceErrorType
```

## Parameters 

`sdRef`  

A pointer to an uninitialized DNSServiceRef. If the call succeeds then it initializes the DNSServiceRef, returns kDNSServiceErr_NoError, and the browse operation will run indefinitely until the client terminates it by passing this DNSServiceRef to DNSServiceRefDeallocate(_:).

`flags`  

Currently ignored, reserved for future use.

`interfaceIndex`  

If non-zero, specifies the interface on which to browse for services (the index for a given interface is determined via the if_nametoindex() family of calls.) Most applications will pass 0 to browse on all available interfaces. See “Constants for specifying an interface index” for more details.

`regtype`  

The service type being browsed for followed by the protocol, separated by a dot (e.g. “\_ftp.\_tcp”). The transport protocol must be “\_tcp” or “\_udp”. A client may optionally specify a single subtype to perform filtered browsing: e.g. browsing for “\_primarytype.\_tcp,\_subtype” will discover only those instances of “\_primarytype.\_tcp” that were registered specifying “\_subtype” in their list of registered subtypes. Additionally, a group identifier may also be specified before the subtype e.g., \_primarytype.\_tcp:GroupID, which will discover only the members that register the service with GroupID. See DNSServiceRegister for more details.

`domain`  

If non-NULL, specifies the domain on which to browse for services. Most applications will not specify a domain, instead browsing on the default domain(s).

`callBack`  

The function to be called when an instance of the service being browsed for is found, or if the call asynchronously fails.

`context`  

An application context pointer which is passed to the callback function (may be NULL).

## Return Value

Returns kDNSServiceErr_NoError on success (any subsequent, asynchronous errors are delivered to the callback), otherwise returns an error code indicating the error that occurred (the callback is not invoked and the DNSServiceRef is not initialized).

## See Also

### Service Discovery

func DNSServiceResolve(UnsafeMutablePointer&lt;DNSServiceRef?>!, DNSServiceFlags, UInt32, UnsafePointer&lt;CChar>!, UnsafePointer&lt;CChar>!, UnsafePointer&lt;CChar>!, DNSServiceResolveReply!, UnsafeMutableRawPointer!) -> DNSServiceErrorType

