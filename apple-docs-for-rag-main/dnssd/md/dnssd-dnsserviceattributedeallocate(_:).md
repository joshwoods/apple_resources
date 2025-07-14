

- dnssd
-  DNSServiceAttributeDeallocate(\_:) 

Function

# DNSServiceAttributeDeallocate(\_:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func DNSServiceAttributeDeallocate(_ attr: DNSServiceAttributeRef)
```

## See Also

### Functions

func DNSServiceSleepKeepalive(UnsafeMutablePointer&lt;DNSServiceRef?>!, DNSServiceFlags, Int32, UInt32, DNSServiceSleepKeepaliveReply!, UnsafeMutableRawPointer!) -> DNSServiceErrorType

func DNSServiceAttributeCreate() -> DNSServiceAttributeRef?

func DNSServiceAttributeSetAAAAPolicy(DNSServiceAttributeRef, DNSServiceAAAAPolicy) -> DNSServiceErrorType

func DNSServiceAttributeSetHostKeyHash(DNSServiceAttributeRef, UInt32) -> DNSServiceErrorType

func DNSServiceAttributeSetTimestamp(DNSServiceAttributeRef, UInt32) -> DNSServiceErrorType

func DNSServiceQueryRecordWithAttribute(UnsafeMutablePointer&lt;DNSServiceRef>?, DNSServiceFlags, UInt32, UnsafePointer&lt;CChar>?, UInt16, UInt16, OpaquePointer?, DNSServiceQueryRecordReply?, UnsafeMutableRawPointer?) -> DNSServiceErrorType

func DNSServiceRegisterRecordWithAttribute(DNSServiceRef?, UnsafeMutablePointer&lt;DNSRecordRef>?, DNSServiceFlags, UInt32, UnsafePointer&lt;CChar>?, UInt16, UInt16, UInt16, UnsafeRawPointer?, UInt32, DNSServiceAttributeRef?, DNSServiceRegisterRecordReply?, UnsafeMutableRawPointer?) -> DNSServiceErrorType

func DNSServiceRegisterWithAttribute(UnsafeMutablePointer&lt;DNSServiceRef>?, DNSServiceFlags, UInt32, UnsafePointer&lt;CChar>?, UnsafePointer&lt;CChar>?, UnsafePointer&lt;CChar>?, UnsafePointer&lt;CChar>?, UInt16, UInt16, UnsafeRawPointer?, DNSServiceAttributeRef?, DNSServiceRegisterReply?, UnsafeMutableRawPointer?) -> DNSServiceErrorType

func DNSServiceSendQueuedRequests(DNSServiceRef?) -> DNSServiceErrorType

func DNSServiceUpdateRecordWithAttribute(DNSServiceRef?, DNSRecordRef?, DNSServiceFlags, UInt16, UnsafeRawPointer?, UInt32, DNSServiceAttributeRef?) -> DNSServiceErrorType

