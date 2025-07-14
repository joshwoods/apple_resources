

- dnssd
-  kDNSServiceInterfaceIndexP2P 

Global Variable

# kDNSServiceInterfaceIndexP2P

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var kDNSServiceInterfaceIndexP2P: UInt32 { get }
```

## Discussion

Specific interface indexes are identified via a 32-bit unsigned integer returned by the if_nametoindex() family of calls.

If the client passes 0 for interface index, that means “do the right thing”, which (at present) means, “if the name is in an mDNS local multicast domain (e.g. ‘local.’, ‘254.169.in-addr.arpa.’, ‘{8,9,A,B}.E.F.ip6.arpa.’) then multicast on all applicable interfaces, otherwise send via unicast to the appropriate DNS server.” Normally, most clients will use 0 for interface index to automatically get the default sensible behaviour.

If the client passes a positive interface index, then that indicates to do the operation only on that one specified interface.

If the client passes kDNSServiceInterfaceIndexLocalOnly when registering a service, then that service will be found \*only\* by other local clients on the same machine that are browsing using kDNSServiceInterfaceIndexLocalOnly or kDNSServiceInterfaceIndexAny. If a client has a ‘private’ service, accessible only to other processes running on the same machine, this allows the client to advertise that service in a way such that it does not inadvertently appear in service lists on all the other machines on the network.

If the client passes kDNSServiceInterfaceIndexLocalOnly when browsing then it will find \*all\* records registered on that same local machine. Clients explicitly wishing to discover \*only\* LocalOnly services can accomplish this by inspecting the interfaceIndex of each service reported to their DNSServiceBrowseReply callback function, and discarding those where the interface index is not kDNSServiceInterfaceIndexLocalOnly.

kDNSServiceInterfaceIndexP2P is meaningful only in Browse, QueryRecord, Register, and Resolve operations. It should not be used in other DNSService APIs.

- If kDNSServiceInterfaceIndexP2P is passed to DNSServiceBrowse(_:_:_:_:_:_:_:) or DNSServiceQueryRecord(_:_:_:_:_:_:_:_:), it restricts the operation to P2P.

- If kDNSServiceInterfaceIndexP2P is passed to DNSServiceRegister, it is mapped internally to kDNSServiceInterfaceIndexAny with the kDNSServiceFlagsIncludeP2P set.

- If kDNSServiceInterfaceIndexP2P is passed to DNSServiceResolve(_:_:_:_:_:_:_:_:), it is mapped internally to kDNSServiceInterfaceIndexAny with the kDNSServiceFlagsIncludeP2P set, because resolving a P2P service may create and/or enable an interface whose index is not known a priori. The resolve callback will indicate the index of the interface via which the service can be accessed.

If applications pass kDNSServiceInterfaceIndexAny to DNSServiceBrowse(_:_:_:_:_:_:_:) or DNSServiceQueryRecord(_:_:_:_:_:_:_:_:), they must set the kDNSServiceFlagsIncludeP2P flag to include P2P. In this case, if a service instance or the record being queried is found over P2P, the resulting ADD event will indicate kDNSServiceInterfaceIndexP2P as the interface index.

## See Also

### Constants

var DNS_SD_ORIGINAL_ENCODING_VERSION_NUMBER_MAX: Int32

let kDNSServiceAttributeAAAAFallback: &lt;&lt;error type>>

var kDNSServiceInterfaceIndexAny: Int32

var kDNSServiceInterfaceIndexBLE: UInt32

var kDNSServiceInterfaceIndexInfra: UInt32

var kDNSServiceInterfaceIndexLocalOnly: UInt32

var kDNSServiceInterfaceIndexUnicast: UInt32

var kDNSServiceMaxDomainName: Int32

var kDNSServiceMaxServiceName: Int32

var kDNSServiceProperty_DaemonVersion: String

The daemon version property.

