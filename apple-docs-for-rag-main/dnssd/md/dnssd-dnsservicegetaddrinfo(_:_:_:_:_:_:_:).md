

- dnssd
-  DNSServiceGetAddrInfo(\_:\_:\_:\_:\_:\_:\_:) 

Function

# DNSServiceGetAddrInfo(\_:\_:\_:\_:\_:\_:\_:)

Queries for the IP address of a hostname by using either Multicast or Unicast DNS.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func DNSServiceGetAddrInfo(
    _ sdRef: UnsafeMutablePointer!,
    _ flags: DNSServiceFlags,
    _ interfaceIndex: UInt32,
    _ protocol: DNSServiceProtocol,
    _ hostname: UnsafePointer!,
    _ callBack: DNSServiceGetAddrInfoReply!,
    _ context: UnsafeMutableRawPointer!
) -> DNSServiceErrorType
```

## Parameters 

`sdRef`  

A pointer to an uninitialized DNSServiceRef. If the call succeeds then it initializes the DNSServiceRef, returns kDNSServiceErr_NoError, and the query begins and will last indefinitely until the client terminates the query by passing this DNSServiceRef to DNSServiceRefDeallocate(_:).

`flags`  

kDNSServiceFlagsForceMulticast or kDNSServiceFlagsLongLivedQuery. Pass kDNSServiceFlagsLongLivedQuery to create a “long-lived” unicast query to a unicast DNS server that implements the protocol. This flag has no effect on link-local multicast queries.

`interfaceIndex`  

The interface on which to issue the query. Passing 0 causes the query to be sent on all active interfaces via Multicast or the primary interface via Unicast.

`protocol`  

Pass in kDNSServiceProtocol_IPv4 to look up IPv4 addresses, or kDNSServiceProtocol_IPv6 to look up IPv6 addresses, or both to look up both kinds. If neither flag is set, the system will apply an intelligent heuristic, which is (currently) that it will attempt to look up both, except:

\* If “hostname” is a wide-area unicast DNS hostname (i.e. not a “.local.” name) but this host has no routable IPv6 address, then the call will not try to look up IPv6 addresses for “hostname”, since any addresses it found would be unlikely to be of any use anyway. Similarly, if this host has no routable IPv4 address, the call will not try to look up IPv4 addresses for “hostname”.

`hostname`  

The fully qualified domain name of the host to be queried for.

`callBack`  

The function to be called when the query succeeds or fails asynchronously.

`context`  

An application context pointer which is passed to the callback function (may be NULL).

## Return Value

Returns kDNSServiceErr_NoError on success (any subsequent, asynchronous errors are delivered to the callback), otherwise returns an error code indicating the error that occurred.

