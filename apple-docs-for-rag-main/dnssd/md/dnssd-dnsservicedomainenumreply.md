

- dnssd
-  DNSServiceDomainEnumReply 

Type Alias

# DNSServiceDomainEnumReply

Callback for handling the results of a previous call to DNSServiceEnumerateDomains(_:_:_:_:_:).

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
typealias DNSServiceDomainEnumReply = (DNSServiceRef?, DNSServiceFlags, UInt32, DNSServiceErrorType, UnsafePointer?, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`sdRef`  

The DNSServiceRef initialized by DNSServiceEnumerateDomains(_:_:_:_:_:).

`flags`  

Possible values are:

kDNSServiceFlagsMoreComing

kDNSServiceFlagsAdd

kDNSServiceFlagsDefault

`interfaceIndex`  

Specifies the interface on which the domain exists. (The index for a given interface is determined via the if_nametoindex() family of calls.)

`errorCode`  

Will be kDNSServiceErr_NoError (0) on success, otherwise indicates the failure that occurred (other parameters are undefined if errorCode is nonzero).

`replyDomain`  

The name of the domain.

`context`  

The context pointer passed to DNSServiceEnumerateDomains.

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

typealias DNSServiceNATPortMappingReply

Callback for handling the reply from a previous call to DNSServiceNATPortMappingReply.

