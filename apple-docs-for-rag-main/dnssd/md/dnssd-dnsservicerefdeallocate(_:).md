

- dnssd
-  DNSServiceRefDeallocate(\_:) 

Function

# DNSServiceRefDeallocate(\_:)

Terminates a connection with the daemon and frees memory associated with the DNSServiceRef.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func DNSServiceRefDeallocate(_ sdRef: DNSServiceRef!)
```

## Parameters 

`sdRef`  

A DNSServiceRef initialized by any of the DNSService calls.

## Discussion

Any services or records registered with this DNSServiceRef will be deregistered. Any Browse, Resolve, or Query operations called with this reference will be terminated.

Note: If the reference’s underlying socket is used in a run loop or select() call, it should be removed BEFORE DNSServiceRefDeallocate(_:) is called, as this function closes the reference’s socket.

Note: If the reference was initialized with DNSServiceCreateConnection(_:), any DNSRecordRefs created via this reference will be invalidated by this call - the resource records are deregistered, and their DNSRecordRefs may not be used in subsequent functions. Similarly, if the reference was initialized with DNSServiceRegister(_:_:_:_:_:_:_:_:_:_:_:_:), and an extra resource record was added to the service via DNSServiceAddRecord(_:_:_:_:_:_:_:), the DNSRecordRef created by the add call is invalidated when this function is called - the DNSRecordRef may not be used in subsequent functions.

Note: This call is to be used only with the DNSServiceRef defined by this API.

## See Also

### Unix Domain Socket access, DNSServiceRef deallocation, and data processing functions

func DNSServiceProcessResult(DNSServiceRef!) -> DNSServiceErrorType

Reads a reply from the daemon, calling the appropriate application callback.

func DNSServiceRefSockFD(DNSServiceRef!) -> dnssd_sock_t

Accesses underlying Unix domain socket for an initialized DNSServiceRef.

