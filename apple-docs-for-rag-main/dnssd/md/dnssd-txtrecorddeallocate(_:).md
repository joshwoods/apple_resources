

- dnssd
-  TXTRecordDeallocate(\_:) 

Function

# TXTRecordDeallocate(\_:)

Releases resources associated with a TXT record.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func TXTRecordDeallocate(_ txtRecord: UnsafeMutablePointer!)
```

## Parameters 

`txtRecord`  

A TXTRecordRef initialized by calling TXTRecordCreate().

## Discussion

Releases any resources allocated in the course of preparing a TXT Record using TXTRecordCreate()/TXTRecordSetValue()/TXTRecordRemoveValue(). Ownership of the buffer provided in TXTRecordCreate() returns to the client.

## See Also

### TXT Record Construction Functions

func TXTRecordCreate(UnsafeMutablePointer&lt;TXTRecordRef>!, UInt16, UnsafeMutableRawPointer!)

Creates a new empty TXTRecordRef referencing the specified storage.

func TXTRecordGetBytesPtr(UnsafePointer&lt;TXTRecordRef>!) -> UnsafeRawPointer!

Allows you to retrieve a pointer to the raw bytes within a TXTRecordRef.

func TXTRecordGetLength(UnsafePointer&lt;TXTRecordRef>!) -> UInt16

Allows you to determine the length of the raw bytes within a TXTRecordRef.

func TXTRecordRemoveValue(UnsafeMutablePointer&lt;TXTRecordRef>!, UnsafePointer&lt;CChar>!) -> DNSServiceErrorType

Removes a key from a TXTRecordRef.

func TXTRecordSetValue(UnsafeMutablePointer&lt;TXTRecordRef>!, UnsafePointer&lt;CChar>!, UInt8, UnsafeRawPointer!) -> DNSServiceErrorType

Adds a key (optionally with value) to a TXTRecordRef.

