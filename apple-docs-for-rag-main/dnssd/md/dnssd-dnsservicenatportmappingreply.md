

- dnssd
-  DNSServiceNATPortMappingReply 

Type Alias

# DNSServiceNATPortMappingReply

Callback for handling the reply from a previous call to DNSServiceNATPortMappingReply.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
typealias DNSServiceNATPortMappingReply = (DNSServiceRef?, DNSServiceFlags, UInt32, DNSServiceErrorType, UInt32, DNSServiceProtocol, UInt16, UInt16, UInt32, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`sdRef`  

The DNSServiceRef initialized by DNSServiceNATPortMappingCreate(_:_:_:_:_:_:_:_:_:).

`flags`  

Currently unused, reserved for future use.

`interfaceIndex`  

The interface through which the NAT gateway is reached.

`errorCode`  

Will be kDNSServiceErr_NoError on success. Will be kDNSServiceErr_DoubleNAT when the NAT gateway is itself behind one or more layers of NAT, in which case the other parameters have the defined values. For other failures, will indicate the failure that occurred, and the other parameters are undefined.

`externalAddress`  

Four byte IPv4 address in network byte order.

`protocol`  

Will be kDNSServiceProtocol_UDP or kDNSServiceProtocol_TCP or both.

`internalPort`  

The port on the local machine that was mapped.

`externalPort`  

The actual external port in the NAT gateway that was mapped. This is likely to be different than the requested external port.

`ttl`  

The lifetime of the NAT port mapping created on the gateway. This controls how quickly stale mappings will be garbage-collected if the client machine crashes, suffers a power failure, is disconnected from the network, or suffers some other unfortunate demise which causes it to vanish without explicitly removing its NAT port mapping. It’s possible that the ttl value will differ from the requested ttl value.

`context`  

The context pointer that was passed to the callout.

## Discussion

The NAT should support either the NAT-PMP or the UPnP IGD protocol for this API to create a successful mapping.

## See Also

### Callbacks

typealias DNSServiceGetAddrInfoReply

Callback for handling the results of a previous call to DNSServiceGetAddrInfo(_:_:_:_:_:_:_:).

typealias DNSServiceRegisterRecordReply

Callback for handling the results of a previous call to DNSServiceRegisterRecord(_:_:_:_:_:_:_:_:_:_:_:_:).

typealias DNSServiceRegisterReply

Handler for the results from a previous call to DNSServiceRegister(_:_:_:_:_:_:_:_:_:_:_:_:).

typealias DNSServiceBrowseReply

Callback for handling the results of previous calls to DNSServiceBrowse.

typealias DNSServiceResolveReply

typealias DNSServiceQueryRecordReply

Callback for handling the results of a previous call to DNSServiceQueryRecord(_:_:_:_:_:_:_:_:).

typealias DNSServiceDomainEnumReply

Callback for handling the results of a previous call to DNSServiceEnumerateDomains(_:_:_:_:_:).

