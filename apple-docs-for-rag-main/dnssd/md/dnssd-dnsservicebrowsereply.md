

- dnssd
-  DNSServiceBrowseReply 

Type Alias

# DNSServiceBrowseReply

Callback for handling the results of previous calls to DNSServiceBrowse.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
typealias DNSServiceBrowseReply = (DNSServiceRef?, DNSServiceFlags, UInt32, DNSServiceErrorType, UnsafePointer?, UnsafePointer?, UnsafePointer?, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`sdRef`  

The DNSServiceRef initialized by DNSServiceBrowse(_:_:_:_:_:_:_:).

`flags`  

Possible values are kDNSServiceFlagsMoreComing and kDNSServiceFlagsAdd. See flag definitions for details.

`interfaceIndex`  

The interface on which the service is advertised. This index should be passed to DNSServiceResolve(_:_:_:_:_:_:_:_:) when resolving the service.

`errorCode`  

Will be kDNSServiceErr_NoError (0) on success, otherwise will indicate the failure that occurred. Other parameters are undefined if the errorCode is nonzero.

`serviceName`  

The discovered service name. This name should be displayed to the user, and stored for subsequent use in the DNSServiceResolve(_:_:_:_:_:_:_:_:) call.

`regtype`  

The service type, which is usually (but not always) the same as was passed to DNSServiceBrowse(_:_:_:_:_:_:_:). One case where the discovered service type may not be the same as the requested service type is when using subtypes: The client may want to browse for only those ftp servers that allow anonymous connections. The client will pass the string “\_ftp.\_tcp,\_anon” to DNSServiceBrowse(_:_:_:_:_:_:_:), but the type of the service that’s discovered is simply “\_ftp.\_tcp”. The regtype for each discovered service instance should be stored along with the name, so that it can be passed to DNSServiceResolve(_:_:_:_:_:_:_:_:) when the service is later resolved.

`replyDomain`  

The domain of the discovered service instance. This may or may not be the same as the domain that was passed to DNSServiceBrowse(_:_:_:_:_:_:_:). The domain for each discovered service instance should be stored along with the name, so that it can be passed to DNSServiceResolve(_:_:_:_:_:_:_:_:) when the service is later resolved.

`context`  

The context pointer that was passed to the callout.

## See Also

### Callbacks

typealias DNSServiceGetAddrInfoReply

Callback for handling the results of a previous call to DNSServiceGetAddrInfo(_:_:_:_:_:_:_:).

typealias DNSServiceRegisterRecordReply

Callback for handling the results of a previous call to DNSServiceRegisterRecord(_:_:_:_:_:_:_:_:_:_:_:_:).

typealias DNSServiceRegisterReply

Handler for the results from a previous call to DNSServiceRegister(_:_:_:_:_:_:_:_:_:_:_:_:).

typealias DNSServiceResolveReply

typealias DNSServiceQueryRecordReply

Callback for handling the results of a previous call to DNSServiceQueryRecord(_:_:_:_:_:_:_:_:).

typealias DNSServiceNATPortMappingReply

Callback for handling the reply from a previous call to DNSServiceNATPortMappingReply.

typealias DNSServiceDomainEnumReply

Callback for handling the results of a previous call to DNSServiceEnumerateDomains(_:_:_:_:_:).

