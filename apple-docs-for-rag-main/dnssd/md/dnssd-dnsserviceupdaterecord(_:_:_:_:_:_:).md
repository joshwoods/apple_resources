

- dnssd
-  DNSServiceUpdateRecord(\_:\_:\_:\_:\_:\_:) 

Function

# DNSServiceUpdateRecord(\_:\_:\_:\_:\_:\_:)

Updates a registered resource record.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func DNSServiceUpdateRecord(
    _ sdRef: DNSServiceRef!,
    _ recordRef: DNSRecordRef!,
    _ flags: DNSServiceFlags,
    _ rdlen: UInt16,
    _ rdata: UnsafeRawPointer!,
    _ ttl: UInt32
) -> DNSServiceErrorType
```

## Parameters 

`sdRef`  

A DNSServiceRef that was initialized by DNSServiceRegister(_:_:_:_:_:_:_:_:_:_:_:_:) or DNSServiceCreateConnection(_:).

`recordRef`  

A DNSRecordRef initialized by DNSServiceAddRecord(_:_:_:_:_:_:_:), or NULL to update the service’s primary txt record.

`flags`  

Currently ignored, reserved for future use.

`rdlen`  

The length, in bytes, of the new rdata.

`rdata`  

The new rdata to be contained in the updated resource record.

`ttl`  

The time to live of the updated resource record, in seconds. Most clients should pass 0 to indicate that the system should select a sensible default value.

## Return Value

Returns kDNSServiceErr_NoError on success, otherwise returns an error code indicating the error that occurred.

## Discussion

The record must either be:

- The primary txt record of a service registered via DNSServiceRegister(_:_:_:_:_:_:_:_:_:_:_:_:)

- A record added to a registered service via DNSServiceAddRecord(_:_:_:_:_:_:_:)

- An individual record registered by DNSServiceRegisterRecord(_:_:_:_:_:_:_:_:_:_:_:_:)

## See Also

### Service Registration

func DNSServiceAddRecord(DNSServiceRef!, UnsafeMutablePointer&lt;DNSRecordRef?>!, DNSServiceFlags, UInt16, UInt16, UnsafeRawPointer!, UInt32) -> DNSServiceErrorType

Adds a record to a registered service.

func DNSServiceRegister(UnsafeMutablePointer&lt;DNSServiceRef?>!, DNSServiceFlags, UInt32, UnsafePointer&lt;CChar>!, UnsafePointer&lt;CChar>!, UnsafePointer&lt;CChar>!, UnsafePointer&lt;CChar>!, UInt16, UInt16, UnsafeRawPointer!, DNSServiceRegisterReply!, UnsafeMutableRawPointer!) -> DNSServiceErrorType

Registers a service.

func DNSServiceRemoveRecord(DNSServiceRef!, DNSRecordRef!, DNSServiceFlags) -> DNSServiceErrorType

Removes a record previously added to a service record set via DNSServiceAddRecord(_:_:_:_:_:_:_:), or deregister an record registered individually via DNSServiceRegisterRecord(_:_:_:_:_:_:_:_:_:_:_:_:).

