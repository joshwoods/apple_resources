

- dnssd
-  DNSServiceResolveReply 

Type Alias

# DNSServiceResolveReply

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
typealias DNSServiceResolveReply = (DNSServiceRef?, DNSServiceFlags, UInt32, DNSServiceErrorType, UnsafePointer?, UnsafePointer?, UInt16, UInt16, UnsafePointer?, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`sdRef`  

The DNSServiceRef initialized by DNSServiceResolve(_:_:_:_:_:_:_:_:).

`flags`  

Possible values: kDNSServiceFlagsMoreComing

`interfaceIndex`  

The interface on which the service was resolved.

`errorCode`  

Will be kDNSServiceErr_NoError (0) on success, otherwise will indicate the failure that occurred. Other parameters are undefined if the errorCode is nonzero.

`fullname`  

The full service domain name, in the form \.\.\. (This name is escaped following standard DNS rules, making it suitable for passing to standard system DNS APIs such as res_query(), or to the special-purpose functions included in this API that take fullname parameters. See “Notes on DNS Name Escaping” earlier in this file for more details.)

`hosttarget`  

The target hostname of the machine providing the service. This name can be passed to functions like gethostbyname() to identify the host’s IP address.

`port`  

The port, in network byte order, on which connections are accepted for this service.

`txtLen`  

The length of the txt record, in bytes.

`txtRecord`  

The service’s primary txt record, in standard txt record format.

`context`  

The context pointer that was passed to the callout.

NOTE: In earlier versions of this header file, the txtRecord parameter was declared “const char \*” This is incorrect, since it contains length bytes which are values in the range 0 to 255, not -128 to +127. Depending on your compiler settings, this change may cause signed/unsigned mismatch warnings. These should be fixed by updating your own callback function definition to match the corrected function signature using “const unsigned char \*txtRecord”. Making this change may also fix inadvertent bugs in your callback function, where it could have incorrectly interpreted a length byte with value 250 as being -6 instead, with various bad consequences ranging from incorrect operation to software crashes. If you need to maintain portable code that will compile cleanly with both the old and new versions of this header file, you should update your callback function definition to use the correct unsigned value, and then in the place where you pass your callback function to DNSServiceResolve(_:_:_:_:_:_:_:_:), use a cast to eliminate the compiler warning, e.g.:

DNSServiceResolve(sd, flags, index, name, regtype, domain, (DNSServiceResolveReply)MyCallback, context);

This will ensure that your code compiles cleanly without warnings (and more importantly, works correctly) with both the old header and with the new corrected version.

## Discussion

Resolve a service name discovered via DNSServiceBrowse(_:_:_:_:_:_:_:) to a target host name, port number, and txt record.

Note: Applications should NOT use DNSServiceResolve(_:_:_:_:_:_:_:_:) solely for txt record monitoring - use DNSServiceQueryRecord(_:_:_:_:_:_:_:_:) instead, as it is more efficient for this task.

Note: When the desired results have been returned, the client MUST terminate the resolve by calling DNSServiceRefDeallocate(_:).

Note: DNSServiceResolve(_:_:_:_:_:_:_:_:) behaves correctly for typical services that have a single SRV record and a single TXT record. To resolve non-standard services with multiple SRV or TXT records, DNSServiceQueryRecord(_:_:_:_:_:_:_:_:) should be used.

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

typealias DNSServiceQueryRecordReply

Callback for handling the results of a previous call to DNSServiceQueryRecord(_:_:_:_:_:_:_:_:).

typealias DNSServiceNATPortMappingReply

Callback for handling the reply from a previous call to DNSServiceNATPortMappingReply.

typealias DNSServiceDomainEnumReply

Callback for handling the results of a previous call to DNSServiceEnumerateDomains(_:_:_:_:_:).

