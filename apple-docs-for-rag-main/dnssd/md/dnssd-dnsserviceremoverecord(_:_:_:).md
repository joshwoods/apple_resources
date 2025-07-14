

- dnssd
-  DNSServiceRemoveRecord(\_:\_:\_:) 

Function

# DNSServiceRemoveRecord(\_:\_:\_:)

Removes a record previously added to a service record set via DNSServiceAddRecord(_:_:_:_:_:_:_:), or deregister an record registered individually via DNSServiceRegisterRecord(_:_:_:_:_:_:_:_:_:_:_:_:).

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func DNSServiceRemoveRecord(
    _ sdRef: DNSServiceRef!,
    _ RecordRef: DNSRecordRef!,
    _ flags: DNSServiceFlags
) -> DNSServiceErrorType
```

## Parameters 

`sdRef`  

A DNSServiceRef initialized by DNSServiceRegister(_:_:_:_:_:_:_:_:_:_:_:_:) (if the record being removed was registered via DNSServiceAddRecord(_:_:_:_:_:_:_:)) or by DNSServiceCreateConnection(_:) (if the record being removed was registered via DNSServiceRegisterRecord(_:_:_:_:_:_:_:_:_:_:_:_:)).

`RecordRef`  

A DNSRecordRef initialized by a successful call to DNSServiceAddRecord(_:_:_:_:_:_:_:) or DNSServiceRegisterRecord(_:_:_:_:_:_:_:_:_:_:_:_:).

`flags`  

Currently ignored, reserved for future use.

## Return Value

Returns kDNSServiceErr_NoError on success, otherwise returns an error code indicating the error that occurred.

## See Also

### Service Registration

func DNSServiceAddRecord(DNSServiceRef!, UnsafeMutablePointer&lt;DNSRecordRef?>!, DNSServiceFlags, UInt16, UInt16, UnsafeRawPointer!, UInt32) -> DNSServiceErrorType

Adds a record to a registered service.

func DNSServiceRegister(UnsafeMutablePointer&lt;DNSServiceRef?>!, DNSServiceFlags, UInt32, UnsafePointer&lt;CChar>!, UnsafePointer&lt;CChar>!, UnsafePointer&lt;CChar>!, UnsafePointer&lt;CChar>!, UInt16, UInt16, UnsafeRawPointer!, DNSServiceRegisterReply!, UnsafeMutableRawPointer!) -> DNSServiceErrorType

Registers a service.

func DNSServiceUpdateRecord(DNSServiceRef!, DNSRecordRef!, DNSServiceFlags, UInt16, UnsafeRawPointer!, UInt32) -> DNSServiceErrorType

Updates a registered resource record.

