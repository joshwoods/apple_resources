

- dnssd
-  DNSServiceCreateConnection(\_:) 

Function

# DNSServiceCreateConnection(\_:)

Creates a connection to the daemon, allowing efficient registration of multiple individual records.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func DNSServiceCreateConnection(_ sdRef: UnsafeMutablePointer!) -> DNSServiceErrorType
```

## Parameters 

`sdRef`  

A pointer to an uninitialized DNSServiceRef. Deallocating the reference (via DNSServiceRefDeallocate(_:)) severs the connection and deregisters all records registered on this connection.

## Return Value

Returns kDNSServiceErr_NoError on success, otherwise returns an error code indicating the specific failure that occurred (in which case the DNSServiceRef is not initialized).

## See Also

### Special Purpose Calls

func DNSServiceReconfirmRecord(DNSServiceFlags, UInt32, UnsafePointer&lt;CChar>!, UInt16, UInt16, UInt16, UnsafeRawPointer!) -> DNSServiceErrorType

Instructs the daemon to verify the validity of a resource record that appears to be out of date (for example, because TCP connection to a service’s target failed).

func DNSServiceRegisterRecord(DNSServiceRef!, UnsafeMutablePointer&lt;DNSRecordRef?>!, DNSServiceFlags, UInt32, UnsafePointer&lt;CChar>!, UInt16, UInt16, UInt16, UnsafeRawPointer!, UInt32, DNSServiceRegisterRecordReply!, UnsafeMutableRawPointer!) -> DNSServiceErrorType

Registers an individual resource record on a connected DNSServiceRef.

func PeerConnectionRelease(DNSServiceFlags, UnsafePointer&lt;CChar>!, UnsafePointer&lt;CChar>!, UnsafePointer&lt;CChar>!) -> DNSServiceErrorType

Releases P2P connection resources associated with the service instance.

