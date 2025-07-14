

- dnssd
-  DNSServiceRegisterRecord(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# DNSServiceRegisterRecord(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Registers an individual resource record on a connected DNSServiceRef.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func DNSServiceRegisterRecord(
    _ sdRef: DNSServiceRef!,
    _ RecordRef: UnsafeMutablePointer!,
    _ flags: DNSServiceFlags,
    _ interfaceIndex: UInt32,
    _ fullname: UnsafePointer!,
    _ rrtype: UInt16,
    _ rrclass: UInt16,
    _ rdlen: UInt16,
    _ rdata: UnsafeRawPointer!,
    _ ttl: UInt32,
    _ callBack: DNSServiceRegisterRecordReply!,
    _ context: UnsafeMutableRawPointer!
) -> DNSServiceErrorType
```

## Parameters 

`sdRef`  

A DNSServiceRef initialized by DNSServiceCreateConnection(_:).

`RecordRef`  

A pointer to an uninitialized DNSRecordRef. Upon succesfull completion of this call, this ref may be passed to DNSServiceUpdateRecord(_:_:_:_:_:_:) or DNSServiceRemoveRecord(_:_:_:). (To deregister ALL records registered on a single connected DNSServiceRef and deallocate each of their corresponding DNSServiceRecordRefs, call DNSServiceRefDeallocate(_:)).

`flags`  

Possible values are kDNSServiceFlagsShared or kDNSServiceFlagsUnique (see flag type definitions for details).

`interfaceIndex`  

If non-zero, specifies the interface on which to register the record (the index for a given interface is determined via the if_nametoindex() family of calls.) Passing 0 causes the record to be registered on all interfaces. See “Constants for specifying an interface index” for more details.

`fullname`  

The full domain name of the resource record.

`rrtype`  

The numerical type of the resource record (e.g. kDNSServiceType_PTR, kDNSServiceType_SRV, and so on).

`rrclass`  

The class of the resource record (usually kDNSServiceClass_IN)

`rdlen`  

Length, in bytes, of the rdata.

`rdata`  

A pointer to the raw rdata, as it is to appear in the DNS record.

`ttl`  

The time to live of the resource record, in seconds. Most clients should pass 0 to indicate that the system should select a sensible default value.

`callBack`  

The function to be called when a result is found, or if the call asynchronously fails (e.g. because of a name conflict.)

`context`  

An application context pointer which is passed to the callback function (may be NULL).

## Return Value

Returns kDNSServiceErr_NoError on success (any subsequent, asynchronous errors are delivered to the callback), otherwise returns an error code indicating the error that occurred (the callback is never invoked and the DNSRecordRef is not initialized).

## Discussion

Note that name conflicts occurring for records registered via this call must be handled by the client in the callback.

## See Also

### Special Purpose Calls

func DNSServiceCreateConnection(UnsafeMutablePointer&lt;DNSServiceRef?>!) -> DNSServiceErrorType

Creates a connection to the daemon, allowing efficient registration of multiple individual records.

func DNSServiceReconfirmRecord(DNSServiceFlags, UInt32, UnsafePointer&lt;CChar>!, UInt16, UInt16, UInt16, UnsafeRawPointer!) -> DNSServiceErrorType

Instructs the daemon to verify the validity of a resource record that appears to be out of date (for example, because TCP connection to a service’s target failed).

func PeerConnectionRelease(DNSServiceFlags, UnsafePointer&lt;CChar>!, UnsafePointer&lt;CChar>!, UnsafePointer&lt;CChar>!) -> DNSServiceErrorType

Releases P2P connection resources associated with the service instance.

