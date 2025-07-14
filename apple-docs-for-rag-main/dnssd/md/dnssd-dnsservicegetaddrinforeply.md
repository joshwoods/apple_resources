

- dnssd
-  DNSServiceGetAddrInfoReply 

Type Alias

# DNSServiceGetAddrInfoReply

Callback for handling the results of a previous call to DNSServiceGetAddrInfo(_:_:_:_:_:_:_:).

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
typealias DNSServiceGetAddrInfoReply = (DNSServiceRef?, DNSServiceFlags, UInt32, DNSServiceErrorType, UnsafePointer?, UnsafePointer?, UInt32, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`sdRef`  

The DNSServiceRef initialized by DNSServiceGetAddrInfo(_:_:_:_:_:_:_:).

`flags`  

Possible values are kDNSServiceFlagsMoreComing and kDNSServiceFlagsAdd.

`interfaceIndex`  

The interface to which the answers pertain.

`errorCode`  

Will be kDNSServiceErr_NoError on success, otherwise will indicate the failure that occurred. Other parameters are undefined if errorCode is nonzero.

`hostname`  

The fully qualified domain name of the host to be queried for.

`address`  

IPv4 or IPv6 address.

`ttl`  

If the client wishes to cache the result for performance reasons, the TTL indicates how long the client may legitimately hold onto this result, in seconds. After the TTL expires, the client should consider the result no longer valid, and if it requires this data again, it should be re-fetched with a new query. Of course, this only applies to clients that cancel the asynchronous operation when they get a result. Clients that leave the asynchronous operation running can safely assume that the data remains valid until they get another callback telling them otherwise.

`context`  

The context pointer that was passed to the callout.

## See Also

### Callbacks

typealias DNSServiceRegisterRecordReply

Callback for handling the results of a previous call to DNSServiceRegisterRecord(_:_:_:_:_:_:_:_:_:_:_:_:).

typealias DNSServiceRegisterReply

Handler for the results from a previous call to DNSServiceRegister(_:_:_:_:_:_:_:_:_:_:_:_:).

typealias DNSServiceBrowseReply

Callback for handling the results of previous calls to DNSServiceBrowse.

typealias DNSServiceResolveReply

typealias DNSServiceQueryRecordReply

Callback for handling the results of a previous call to DNSServiceQueryRecord(_:_:_:_:_:_:_:_:).

typealias DNSServiceNATPortMappingReply

Callback for handling the reply from a previous call to DNSServiceNATPortMappingReply.

typealias DNSServiceDomainEnumReply

Callback for handling the results of a previous call to DNSServiceEnumerateDomains(_:_:_:_:_:).

