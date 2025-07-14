

- dnssd
-  DNSServiceSleepKeepalive(\_:\_:\_:\_:\_:\_:) 

Function

# DNSServiceSleepKeepalive(\_:\_:\_:\_:\_:\_:)

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func DNSServiceSleepKeepalive(
    _ sdRef: UnsafeMutablePointer!,
    _ flags: DNSServiceFlags,
    _ fd: Int32,
    _ timeout: UInt32,
    _ callBack: DNSServiceSleepKeepaliveReply!,
    _ context: UnsafeMutableRawPointer!
) -> DNSServiceErrorType
```

## See Also

### Functions

func DNSServiceAttributeCreate() -> DNSServiceAttributeRef?

func DNSServiceAttributeDeallocate(DNSServiceAttributeRef)

func DNSServiceAttributeSetAAAAPolicy(DNSServiceAttributeRef, DNSServiceAAAAPolicy) -> DNSServiceErrorType

func DNSServiceAttributeSetHostKeyHash(DNSServiceAttributeRef, UInt32) -> DNSServiceErrorType

func DNSServiceAttributeSetTimestamp(DNSServiceAttributeRef, UInt32) -> DNSServiceErrorType

func DNSServiceQueryRecordWithAttribute(UnsafeMutablePointer&lt;DNSServiceRef>?, DNSServiceFlags, UInt32, UnsafePointer&lt;CChar>?, UInt16, UInt16, OpaquePointer?, DNSServiceQueryRecordReply?, UnsafeMutableRawPointer?) -> DNSServiceErrorType

func DNSServiceRegisterRecordWithAttribute(DNSServiceRef?, UnsafeMutablePointer&lt;DNSRecordRef>?, DNSServiceFlags, UInt32, UnsafePointer&lt;CChar>?, UInt16, UInt16, UInt16, UnsafeRawPointer?, UInt32, DNSServiceAttributeRef?, DNSServiceRegisterRecordReply?, UnsafeMutableRawPointer?) -> DNSServiceErrorType

func DNSServiceRegisterWithAttribute(UnsafeMutablePointer&lt;DNSServiceRef>?, DNSServiceFlags, UInt32, UnsafePointer&lt;CChar>?, UnsafePointer&lt;CChar>?, UnsafePointer&lt;CChar>?, UnsafePointer&lt;CChar>?, UInt16, UInt16, UnsafeRawPointer?, DNSServiceAttributeRef?, DNSServiceRegisterReply?, UnsafeMutableRawPointer?) -> DNSServiceErrorType

func DNSServiceSendQueuedRequests(DNSServiceRef?) -> DNSServiceErrorType

func DNSServiceUpdateRecordWithAttribute(DNSServiceRef?, DNSRecordRef?, DNSServiceFlags, UInt16, UnsafeRawPointer?, UInt32, DNSServiceAttributeRef?) -> DNSServiceErrorType

