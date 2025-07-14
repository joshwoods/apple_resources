

- dnssd
-  DNS Service Discovery C 

API Collection

# DNS Service Discovery C

See the Overview section above for header-level documentation.

### Overview

#### Included Headers

- types.h

- types.h

- “Tiano.h”

- \

- \

- \

## Topics

### Version checking

func DNSServiceGetProperty(UnsafePointer&lt;CChar>!, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;UInt32>!) -> DNSServiceErrorType

Gets the specified property of a service.

### Unix Domain Socket access, DNSServiceRef deallocation, and data processing functions

func DNSServiceProcessResult(DNSServiceRef!) -> DNSServiceErrorType

Reads a reply from the daemon, calling the appropriate application callback.

func DNSServiceRefDeallocate(DNSServiceRef!)

Terminates a connection with the daemon and frees memory associated with the DNSServiceRef.

func DNSServiceRefSockFD(DNSServiceRef!) -> dnssd_sock_t

Accesses underlying Unix domain socket for an initialized DNSServiceRef.

### Unified lookup of both IPv4 and IPv6 addresses for a fully qualified hostname

func DNSServiceGetAddrInfo(UnsafeMutablePointer&lt;DNSServiceRef?>!, DNSServiceFlags, UInt32, DNSServiceProtocol, UnsafePointer&lt;CChar>!, DNSServiceGetAddrInfoReply!, UnsafeMutableRawPointer!) -> DNSServiceErrorType

Queries for the IP address of a hostname by using either Multicast or Unicast DNS.

### TXT Record Parsing Functions

A typical calling sequence for TXT record parsing is something like:

## Discussion

Receive TXT record data in DNSServiceResolve(_:_:_:_:_:_:_:_:) callback

```
```

If you wish to retain the values after return from the DNSServiceResolve(_:_:_:_:_:_:_:_:) callback, then you need to copy the data to your own storage using memcpy() or similar, as shown in the example above.

If for some reason you need to parse a TXT record you built yourself using the TXT record construction functions above, then you can do that using TXTRecordGetLength and TXTRecordGetBytesPtr calls: TXTRecordGetValue(TXTRecordGetLength(x), TXTRecordGetBytesPtr(x), key, &len);

Most applications only fetch keys they know about from a TXT record and ignore the rest. However, some debugging tools wish to fetch and display all keys. To do that, use the TXTRecordGetCount() and TXTRecordGetItemAtIndex() calls.

DNSServiceCreateDelegateConnection

Create a delegate connection to the daemon allowing efficient registration of multiple individual records.

func DNSServiceSetDispatchQueue(DNSServiceRef!, dispatch_queue_t!) -> DNSServiceErrorType

Allows you to schedule a DNSServiceRef on a serial dispatch queue for receiving asynchronous callbacks.

func TXTRecordContainsKey(UInt16, UnsafeRawPointer!, UnsafePointer&lt;CChar>!) -> Int32

Allows you to determine if a given TXT Record contains a specified key.

func TXTRecordGetCount(UInt16, UnsafeRawPointer!) -> UInt16

Returns the number of keys stored in the TXT Record.

func TXTRecordGetItemAtIndex(UInt16, UnsafeRawPointer!, UInt16, UInt16, UnsafeMutablePointer&lt;CChar>!, UnsafeMutablePointer&lt;UInt8>!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!) -> DNSServiceErrorType

Allows you to retrieve a key name and value pointer, given an index into a TXT Record.

func TXTRecordGetValuePtr(UInt16, UnsafeRawPointer!, UnsafePointer&lt;CChar>!, UnsafeMutablePointer&lt;UInt8>!) -> UnsafeRawPointer!

Allows you to retrieve the value for a given key from a TXT Record.

### TXT Record Construction Functions

func TXTRecordCreate(UnsafeMutablePointer&lt;TXTRecordRef>!, UInt16, UnsafeMutableRawPointer!)

Creates a new empty TXTRecordRef referencing the specified storage.

func TXTRecordDeallocate(UnsafeMutablePointer&lt;TXTRecordRef>!)

Releases resources associated with a TXT record.

func TXTRecordGetBytesPtr(UnsafePointer&lt;TXTRecordRef>!) -> UnsafeRawPointer!

Allows you to retrieve a pointer to the raw bytes within a TXTRecordRef.

func TXTRecordGetLength(UnsafePointer&lt;TXTRecordRef>!) -> UInt16

Allows you to determine the length of the raw bytes within a TXTRecordRef.

func TXTRecordRemoveValue(UnsafeMutablePointer&lt;TXTRecordRef>!, UnsafePointer&lt;CChar>!) -> DNSServiceErrorType

Removes a key from a TXTRecordRef.

func TXTRecordSetValue(UnsafeMutablePointer&lt;TXTRecordRef>!, UnsafePointer&lt;CChar>!, UInt8, UnsafeRawPointer!) -> DNSServiceErrorType

Adds a key (optionally with value) to a TXTRecordRef.

### Special Purpose Calls

DNSServiceCreateConnection(_:), DNSServiceRegisterRecord(_:_:_:_:_:_:_:_:_:_:_:_:), DNSServiceReconfirmRecord(_:_:_:_:_:_:_:) (most applications will not use these)

func DNSServiceCreateConnection(UnsafeMutablePointer&lt;DNSServiceRef?>!) -> DNSServiceErrorType

Creates a connection to the daemon, allowing efficient registration of multiple individual records.

func DNSServiceReconfirmRecord(DNSServiceFlags, UInt32, UnsafePointer&lt;CChar>!, UInt16, UInt16, UInt16, UnsafeRawPointer!) -> DNSServiceErrorType

Instructs the daemon to verify the validity of a resource record that appears to be out of date (for example, because TCP connection to a service’s target failed).

func DNSServiceRegisterRecord(DNSServiceRef!, UnsafeMutablePointer&lt;DNSRecordRef?>!, DNSServiceFlags, UInt32, UnsafePointer&lt;CChar>!, UInt16, UInt16, UInt16, UnsafeRawPointer!, UInt32, DNSServiceRegisterRecordReply!, UnsafeMutableRawPointer!) -> DNSServiceErrorType

Registers an individual resource record on a connected DNSServiceRef.

func PeerConnectionRelease(DNSServiceFlags, UnsafePointer&lt;CChar>!, UnsafePointer&lt;CChar>!, UnsafePointer&lt;CChar>!) -> DNSServiceErrorType

Releases P2P connection resources associated with the service instance.

### Service Registration

func DNSServiceAddRecord(DNSServiceRef!, UnsafeMutablePointer&lt;DNSRecordRef?>!, DNSServiceFlags, UInt16, UInt16, UnsafeRawPointer!, UInt32) -> DNSServiceErrorType

Adds a record to a registered service.

func DNSServiceRegister(UnsafeMutablePointer&lt;DNSServiceRef?>!, DNSServiceFlags, UInt32, UnsafePointer&lt;CChar>!, UnsafePointer&lt;CChar>!, UnsafePointer&lt;CChar>!, UnsafePointer&lt;CChar>!, UInt16, UInt16, UnsafeRawPointer!, DNSServiceRegisterReply!, UnsafeMutableRawPointer!) -> DNSServiceErrorType

Registers a service.

func DNSServiceRemoveRecord(DNSServiceRef!, DNSRecordRef!, DNSServiceFlags) -> DNSServiceErrorType

Removes a record previously added to a service record set via DNSServiceAddRecord(_:_:_:_:_:_:_:), or deregister an record registered individually via DNSServiceRegisterRecord(_:_:_:_:_:_:_:_:_:_:_:_:).

func DNSServiceUpdateRecord(DNSServiceRef!, DNSRecordRef!, DNSServiceFlags, UInt16, UnsafeRawPointer!, UInt32) -> DNSServiceErrorType

Updates a registered resource record.

### Service Discovery

func DNSServiceBrowse(UnsafeMutablePointer&lt;DNSServiceRef?>!, DNSServiceFlags, UInt32, UnsafePointer&lt;CChar>!, UnsafePointer&lt;CChar>!, DNSServiceBrowseReply!, UnsafeMutableRawPointer!) -> DNSServiceErrorType

Browses for available services.

func DNSServiceResolve(UnsafeMutablePointer&lt;DNSServiceRef?>!, DNSServiceFlags, UInt32, UnsafePointer&lt;CChar>!, UnsafePointer&lt;CChar>!, UnsafePointer&lt;CChar>!, DNSServiceResolveReply!, UnsafeMutableRawPointer!) -> DNSServiceErrorType

### Querying Individual Specific Records

func DNSServiceQueryRecord(UnsafeMutablePointer&lt;DNSServiceRef?>!, DNSServiceFlags, UInt32, UnsafePointer&lt;CChar>!, UInt16, UInt16, DNSServiceQueryRecordReply!, UnsafeMutableRawPointer!) -> DNSServiceErrorType

Query for an arbitrary DNS record.

### NAT Port Mapping

func DNSServiceNATPortMappingCreate(UnsafeMutablePointer&lt;DNSServiceRef?>!, DNSServiceFlags, UInt32, DNSServiceProtocol, UInt16, UInt16, UInt32, DNSServiceNATPortMappingReply!, UnsafeMutableRawPointer!) -> DNSServiceErrorType

Requests a port mapping in the NAT gateway, which maps a port on the local machine to an external port on the NAT.

### General Utility Functions

func DNSServiceConstructFullName(UnsafeMutablePointer&lt;CChar>!, UnsafePointer&lt;CChar>!, UnsafePointer&lt;CChar>!, UnsafePointer&lt;CChar>!) -> DNSServiceErrorType

Concatenates a three-part domain name (as returned by the above callbacks) into a properly-escaped full domain name.

### Domain Enumeration

func DNSServiceEnumerateDomains(UnsafeMutablePointer&lt;DNSServiceRef?>!, DNSServiceFlags, UInt32, DNSServiceDomainEnumReply!, UnsafeMutableRawPointer!) -> DNSServiceErrorType

Enumerates domains that are recommended for registration and browsing.

### Callbacks

See the Overview section above for header-level documentation.

## Discussion

DNSServiceCreateConnection(_:), DNSServiceRegisterRecord(_:_:_:_:_:_:_:_:_:_:_:_:), DNSServiceReconfirmRecord(_:_:_:_:_:_:_:) (most applications will not use these)

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

typealias DNSServiceDomainEnumReply

Callback for handling the results of a previous call to DNSServiceEnumerateDomains(_:_:_:_:_:).

### Data Types

See the Overview section above for header-level documentation.

typealias DNSServiceErrorType

typealias DNSServiceFlags

typealias DNSServiceProtocol

typealias TXTRecordRef

Opaque internal data type that represents a DNS-SD TXT record.

### Constants

See the Overview section above for header-level documentation.

Constants for specifying an interface index

Miscellaneous Defines

## See Also

### Reference

dnssd Enumerations

dnssd Functions

dnssd Data Types

dnssd Constants

