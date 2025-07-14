

- dnssd
-  TXTRecordRemoveValue(\_:\_:) 

Function

# TXTRecordRemoveValue(\_:\_:)

Removes a key from a TXTRecordRef.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func TXTRecordRemoveValue(
    _ txtRecord: UnsafeMutablePointer!,
    _ key: UnsafePointer!
) -> DNSServiceErrorType
```

## Parameters 

`txtRecord`  

A TXTRecordRef initialized by calling TXTRecordCreate().

`key`  

A key name. This value must be an ASCII string that exists in the TXTRecordRef.

## Return Value

Returns kDNSServiceErr_NoError on success. Returns kDNSServiceErr_NoSuchKey if the “key” does not exist in the TXTRecordRef.

## See Also

### TXT Record Construction Functions

func TXTRecordCreate(UnsafeMutablePointer&lt;TXTRecordRef>!, UInt16, UnsafeMutableRawPointer!)

Creates a new empty TXTRecordRef referencing the specified storage.

func TXTRecordDeallocate(UnsafeMutablePointer&lt;TXTRecordRef>!)

Releases resources associated with a TXT record.

func TXTRecordGetBytesPtr(UnsafePointer&lt;TXTRecordRef>!) -> UnsafeRawPointer!

Allows you to retrieve a pointer to the raw bytes within a TXTRecordRef.

func TXTRecordGetLength(UnsafePointer&lt;TXTRecordRef>!) -> UInt16

Allows you to determine the length of the raw bytes within a TXTRecordRef.

func TXTRecordSetValue(UnsafeMutablePointer&lt;TXTRecordRef>!, UnsafePointer&lt;CChar>!, UInt8, UnsafeRawPointer!) -> DNSServiceErrorType

Adds a key (optionally with value) to a TXTRecordRef.

