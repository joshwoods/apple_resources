

- dnssd
-  PeerConnectionRelease(\_:\_:\_:\_:) 

Function

# PeerConnectionRelease(\_:\_:\_:\_:)

Releases P2P connection resources associated with the service instance.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func PeerConnectionRelease(
    _ flags: DNSServiceFlags,
    _ name: UnsafePointer!,
    _ regtype: UnsafePointer!,
    _ domain: UnsafePointer!
) -> DNSServiceErrorType
```

## Discussion

When a service is resolved over a P2P interface, a connection is brought up to the peer advertising the service instance. This call will free the resources associated with that connection. Note that the reference to the service instance will only be maintained by the mDNSResponder daemon while the browse for the service type is still running. Thus the sequence of calls to discover, resolve, and then terminate the connection associated with a given P2P service instance would be:

DNSServiceRef BrowseRef, ResolveRef; DNSServiceBrowse(&BrowseRef, …) // browse for all instances of the service DNSServiceResolve(&ResolveRef, …) // resolving a service instance creates a // connection to the peer device advertising that service DNSServiceRefDeallocate(ResolveRef) // Stop the resolve, which does not close the peer connection

// Communicate with the peer application.

PeerConnectionRelease() // release the connection to the peer device for the specified service instance

DNSServiceRefDeallocate(BrowseRef) // stop the browse // Any further calls to PeerConnectionRelease() will have no affect since the // service instance to peer connection relationship is only maintained by the // mDNSResponder daemon while the browse is running.

flags: Not currently used.

name: The name of the service instance to be resolved, as reported to the DNSServiceBrowseReply callback.

regtype: The type of the service instance to be resolved, as reported to the DNSServiceBrowseReply callback.

domain: The domain of the service instance to be resolved, as reported to the DNSServiceBrowseReply callback.

return value: Returns kDNSServiceErr_NoError on success or the error that occurred.

## See Also

### Special Purpose Calls

func DNSServiceCreateConnection(UnsafeMutablePointer&lt;DNSServiceRef?>!) -> DNSServiceErrorType

Creates a connection to the daemon, allowing efficient registration of multiple individual records.

func DNSServiceReconfirmRecord(DNSServiceFlags, UInt32, UnsafePointer&lt;CChar>!, UInt16, UInt16, UInt16, UnsafeRawPointer!) -> DNSServiceErrorType

Instructs the daemon to verify the validity of a resource record that appears to be out of date (for example, because TCP connection to a service’s target failed).

func DNSServiceRegisterRecord(DNSServiceRef!, UnsafeMutablePointer&lt;DNSRecordRef?>!, DNSServiceFlags, UInt32, UnsafePointer&lt;CChar>!, UInt16, UInt16, UInt16, UnsafeRawPointer!, UInt32, DNSServiceRegisterRecordReply!, UnsafeMutableRawPointer!) -> DNSServiceErrorType

Registers an individual resource record on a connected DNSServiceRef.

