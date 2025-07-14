

- dnssd
-  dnssd Functions 

API Collection

# dnssd Functions

## Topics

### Functions

func DNSServiceSleepKeepalive(UnsafeMutablePointer&lt;DNSServiceRef?>!, DNSServiceFlags, Int32, UInt32, DNSServiceSleepKeepaliveReply!, UnsafeMutableRawPointer!) -> DNSServiceErrorType

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

## See Also

### Reference

DNS Service Discovery C

See the Overview section above for header-level documentation.

dnssd Enumerations

dnssd Data Types

dnssd Constants

