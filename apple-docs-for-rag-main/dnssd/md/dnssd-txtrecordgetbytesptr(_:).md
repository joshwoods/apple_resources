

- dnssd
-  TXTRecordGetBytesPtr(\_:) 

Function

# TXTRecordGetBytesPtr(\_:)

Allows you to retrieve a pointer to the raw bytes within a TXTRecordRef.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func TXTRecordGetBytesPtr(_ txtRecord: UnsafePointer!) -> UnsafeRawPointer!
```

## Parameters 

`txtRecord`  

A TXTRecordRef initialized by calling TXTRecordCreate().

## Return Value

Returns a pointer to the raw bytes inside the TXTRecordRef which you can pass directly to DNSServiceRegister(_:_:_:_:_:_:_:_:_:_:_:_:) or to DNSServiceUpdateRecord(_:_:_:_:_:_:).

## See Also

### TXT Record Construction Functions

func TXTRecordCreate(UnsafeMutablePointer&lt;TXTRecordRef>!, UInt16, UnsafeMutableRawPointer!)

Creates a new empty TXTRecordRef referencing the specified storage.

func TXTRecordDeallocate(UnsafeMutablePointer&lt;TXTRecordRef>!)

Releases resources associated with a TXT record.

func TXTRecordGetLength(UnsafePointer&lt;TXTRecordRef>!) -> UInt16

Allows you to determine the length of the raw bytes within a TXTRecordRef.

func TXTRecordRemoveValue(UnsafeMutablePointer&lt;TXTRecordRef>!, UnsafePointer&lt;CChar>!) -> DNSServiceErrorType

Removes a key from a TXTRecordRef.

func TXTRecordSetValue(UnsafeMutablePointer&lt;TXTRecordRef>!, UnsafePointer&lt;CChar>!, UInt8, UnsafeRawPointer!) -> DNSServiceErrorType

Adds a key (optionally with value) to a TXTRecordRef.

