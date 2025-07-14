

- dnssd
-  DNSServiceRegisterRecordWithAttribute(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# DNSServiceRegisterRecordWithAttribute(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func DNSServiceRegisterRecordWithAttribute(
    _ sdRef: DNSServiceRef?,
    _ recordRef: UnsafeMutablePointer?,
    _ flags: DNSServiceFlags,
    _ interfaceIndex: UInt32,
    _ fullname: UnsafePointer?,
    _ rrtype: UInt16,
    _ rrclass: UInt16,
    _ rdlen: UInt16,
    _ rdata: UnsafeRawPointer?,
    _ ttl: UInt32,
    _ attr: DNSServiceAttributeRef?,
    _ callBack: DNSServiceRegisterRecordReply?,
    _ context: UnsafeMutableRawPointer?
) -> DNSServiceErrorType
```

## See Also

### Functions

func DNSServiceSleepKeepalive(UnsafeMutablePointer&lt;DNSServiceRef?>!, DNSServiceFlags, Int32, UInt32, DNSServiceSleepKeepaliveReply!, UnsafeMutableRawPointer!) -> DNSServiceErrorType

func DNSServiceAttributeCreate() -> DNSServiceAttributeRef?

func DNSServiceAttributeDeallocate(DNSServiceAttributeRef)

func DNSServiceAttributeSetAAAAPolicy(DNSServiceAttributeRef, DNSServiceAAAAPolicy) -> DNSServiceErrorType

func DNSServiceAttributeSetHostKeyHash(DNSServiceAttributeRef, UInt32) -> DNSServiceErrorType

func DNSServiceAttributeSetTimestamp(DNSServiceAttributeRef, UInt32) -> DNSServiceErrorType

func DNSServiceQueryRecordWithAttribute(UnsafeMutablePointer&lt;DNSServiceRef>?, DNSServiceFlags, UInt32, UnsafePointer&lt;CChar>?, UInt16, UInt16, OpaquePointer?, DNSServiceQueryRecordReply?, UnsafeMutableRawPointer?) -> DNSServiceErrorType

func DNSServiceRegisterWithAttribute(UnsafeMutablePointer&lt;DNSServiceRef>?, DNSServiceFlags, UInt32, UnsafePointer&lt;CChar>?, UnsafePointer&lt;CChar>?, UnsafePointer&lt;CChar>?, UnsafePointer&lt;CChar>?, UInt16, UInt16, UnsafeRawPointer?, DNSServiceAttributeRef?, DNSServiceRegisterReply?, UnsafeMutableRawPointer?) -> DNSServiceErrorType

func DNSServiceSendQueuedRequests(DNSServiceRef?) -> DNSServiceErrorType

func DNSServiceUpdateRecordWithAttribute(DNSServiceRef?, DNSRecordRef?, DNSServiceFlags, UInt16, UnsafeRawPointer?, UInt32, DNSServiceAttributeRef?) -> DNSServiceErrorType

