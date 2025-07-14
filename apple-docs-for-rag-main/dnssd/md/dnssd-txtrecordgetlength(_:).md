

- dnssd
-  TXTRecordGetLength(\_:) 

Function

# TXTRecordGetLength(\_:)

Allows you to determine the length of the raw bytes within a TXTRecordRef.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func TXTRecordGetLength(_ txtRecord: UnsafePointer!) -> UInt16
```

## Parameters 

`txtRecord`  

A TXTRecordRef initialized by calling TXTRecordCreate().

## Return Value

Returns the size of the raw bytes inside a TXTRecordRef which you can pass directly to DNSServiceRegister(_:_:_:_:_:_:_:_:_:_:_:_:) or to DNSServiceUpdateRecord(_:_:_:_:_:_:). Returns 0 if the TXTRecordRef is empty.

## See Also

### TXT Record Construction Functions

func TXTRecordCreate(UnsafeMutablePointer&lt;TXTRecordRef>!, UInt16, UnsafeMutableRawPointer!)

Creates a new empty TXTRecordRef referencing the specified storage.

func TXTRecordDeallocate(UnsafeMutablePointer&lt;TXTRecordRef>!)

Releases resources associated with a TXT record.

func TXTRecordGetBytesPtr(UnsafePointer&lt;TXTRecordRef>!) -> UnsafeRawPointer!

Allows you to retrieve a pointer to the raw bytes within a TXTRecordRef.

func TXTRecordRemoveValue(UnsafeMutablePointer&lt;TXTRecordRef>!, UnsafePointer&lt;CChar>!) -> DNSServiceErrorType

Removes a key from a TXTRecordRef.

func TXTRecordSetValue(UnsafeMutablePointer&lt;TXTRecordRef>!, UnsafePointer&lt;CChar>!, UInt8, UnsafeRawPointer!) -> DNSServiceErrorType

Adds a key (optionally with value) to a TXTRecordRef.

