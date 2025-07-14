

- dnssd
-  DNSServiceProcessResult(\_:) 

Function

# DNSServiceProcessResult(\_:)

Reads a reply from the daemon, calling the appropriate application callback.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func DNSServiceProcessResult(_ sdRef: DNSServiceRef!) -> DNSServiceErrorType
```

## Parameters 

`sdRef`  

A DNSServiceRef initialized by any of the DNSService calls that take a callback parameter.

## Return Value

Returns kDNSServiceErr_NoError on success, otherwise returns an error code indicating the specific failure that occurred.

## Discussion

This call blocks until the daemon’s response is received. Use DNSServiceRefSockFD(_:) in conjunction with a run loop or select() to determine the presence of a response from the server before calling this function to process the reply without blocking. Call this function at any point if it is acceptable to block until the daemon’s response arrives. Note that the client is responsible for ensuring that DNSServiceProcessResult(_:) is called whenever there is a reply from the daemon - the daemon may terminate its connection with a client that does not process the daemon’s responses.

## See Also

### Unix Domain Socket access, DNSServiceRef deallocation, and data processing functions

func DNSServiceRefDeallocate(DNSServiceRef!)

Terminates a connection with the daemon and frees memory associated with the DNSServiceRef.

func DNSServiceRefSockFD(DNSServiceRef!) -> dnssd_sock_t

Accesses underlying Unix domain socket for an initialized DNSServiceRef.

