

- dnssd
-  DNSServiceReconfirmRecord(\_:\_:\_:\_:\_:\_:\_:) 

Function

# DNSServiceReconfirmRecord(\_:\_:\_:\_:\_:\_:\_:)

Instructs the daemon to verify the validity of a resource record that appears to be out of date (for example, because TCP connection to a service’s target failed).

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func DNSServiceReconfirmRecord(
    _ flags: DNSServiceFlags,
    _ interfaceIndex: UInt32,
    _ fullname: UnsafePointer!,
    _ rrtype: UInt16,
    _ rrclass: UInt16,
    _ rdlen: UInt16,
    _ rdata: UnsafeRawPointer!
) -> DNSServiceErrorType
```

## Parameters 

`flags`  

Not currently used.

`interfaceIndex`  

Specifies the interface of the record in question. The caller must specify the interface. This API (by design) causes increased network traffic, so it requires the caller to be precise about which record should be reconfirmed. It is not possible to pass zero for the interface index to perform a “wildcard” reconfirmation, where \*all\* matching records are reconfirmed.

`fullname`  

The resource record’s full domain name.

`rrtype`  

The resource record’s type (e.g. kDNSServiceType_PTR, kDNSServiceType_SRV, and so on).

`rrclass`  

The class of the resource record (usually kDNSServiceClass_IN).

`rdlen`  

The length, in bytes, of the resource record rdata.

`rdata`  

The raw rdata of the resource record.

## Discussion

Causes the record to be flushed from the daemon’s cache (as well as all other daemons’ caches on the network) if the record is determined to be invalid.

Important

Use this routine conservatively. Reconfirming a record necessarily consumes network bandwidth, so this should not be done indiscriminately.

## See Also

### Special Purpose Calls

func DNSServiceCreateConnection(UnsafeMutablePointer&lt;DNSServiceRef?>!) -> DNSServiceErrorType

Creates a connection to the daemon, allowing efficient registration of multiple individual records.

func DNSServiceRegisterRecord(DNSServiceRef!, UnsafeMutablePointer&lt;DNSRecordRef?>!, DNSServiceFlags, UInt32, UnsafePointer&lt;CChar>!, UInt16, UInt16, UInt16, UnsafeRawPointer!, UInt32, DNSServiceRegisterRecordReply!, UnsafeMutableRawPointer!) -> DNSServiceErrorType

Registers an individual resource record on a connected DNSServiceRef.

func PeerConnectionRelease(DNSServiceFlags, UnsafePointer&lt;CChar>!, UnsafePointer&lt;CChar>!, UnsafePointer&lt;CChar>!) -> DNSServiceErrorType

Releases P2P connection resources associated with the service instance.

