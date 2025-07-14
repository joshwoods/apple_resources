

- dnssd
-  DNSServiceRegisterRecordReply 

Type Alias

# DNSServiceRegisterRecordReply

Callback for handling the results of a previous call to DNSServiceRegisterRecord(_:_:_:_:_:_:_:_:_:_:_:_:).

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
typealias DNSServiceRegisterRecordReply = (DNSServiceRef?, DNSRecordRef?, DNSServiceFlags, DNSServiceErrorType, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`sdRef`  

The connected DNSServiceRef initialized by DNSServiceCreateConnection(_:).

`RecordRef`  

The DNSRecordRef initialized by DNSServiceRegisterRecord(_:_:_:_:_:_:_:_:_:_:_:_:). If the above DNSServiceRef is passed to DNSServiceRefDeallocate(_:), this DNSRecordRef is invalidated, and may not be used further.

`flags`  

Currently unused, reserved for future use.

`errorCode`  

Will be kDNSServiceErr_NoError on success, otherwise will indicate the failure that occurred (including name conflicts.) Other parameters are undefined if errorCode is nonzero.

`context`  

The context pointer that was passed to the callout.

## See Also

### Callbacks

typealias DNSServiceGetAddrInfoReply

Callback for handling the results of a previous call to DNSServiceGetAddrInfo(_:_:_:_:_:_:_:).

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

