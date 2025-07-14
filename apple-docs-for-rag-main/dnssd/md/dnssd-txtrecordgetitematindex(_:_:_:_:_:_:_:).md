

- dnssd
-  TXTRecordGetItemAtIndex(\_:\_:\_:\_:\_:\_:\_:) 

Function

# TXTRecordGetItemAtIndex(\_:\_:\_:\_:\_:\_:\_:)

Allows you to retrieve a key name and value pointer, given an index into a TXT Record.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func TXTRecordGetItemAtIndex(
    _ txtLen: UInt16,
    _ txtRecord: UnsafeRawPointer!,
    _ itemIndex: UInt16,
    _ keyBufLen: UInt16,
    _ key: UnsafeMutablePointer!,
    _ valueLen: UnsafeMutablePointer!,
    _ value: UnsafeMutablePointer!
) -> DNSServiceErrorType
```

## Parameters 

`txtLen`  

The size of the received TXT Record.

`txtRecord`  

Pointer to the received TXT Record bytes.

`itemIndex`  

An index into the TXT Record.

`keyBufLen`  

The size of the string buffer being supplied.

`key`  

A string buffer used to store the key name. On return, the buffer contains a null-terminated C string giving the key name. DNS-SD TXT keys are usually 9 characters or fewer. To hold the maximum possible key name, the buffer should be 256 bytes long.

`valueLen`  

On output, will be set to the size of the “value” data.

`value`  

On output, \*value is set to point to location within TXT Record bytes that holds the value data.

## Return Value

Returns kDNSServiceErr_NoError on success. Returns kDNSServiceErr_NoMemory if keyBufLen is too short. Returns kDNSServiceErr_Invalid if index is greater than TXTRecordGetCount()-1.

## Discussion

Legal index values range from zero to TXTRecordGetCount()-1. It’s also possible to iterate through keys in a TXT record by simply calling TXTRecordGetItemAtIndex() repeatedly, beginning with index zero and increasing until TXTRecordGetItemAtIndex() returns kDNSServiceErr_Invalid.

On return:

For keys with no value, \*value is set to NULL and \*valueLen is zero.

For keys with empty value, \*value is non-NULL and \*valueLen is zero.

For keys with non-empty value, \*value is non-NULL and \*valueLen is non-zero.

## See Also

### TXT Record Parsing Functions

DNSServiceCreateDelegateConnection

Create a delegate connection to the daemon allowing efficient registration of multiple individual records.

func DNSServiceSetDispatchQueue(DNSServiceRef!, dispatch_queue_t!) -> DNSServiceErrorType

Allows you to schedule a DNSServiceRef on a serial dispatch queue for receiving asynchronous callbacks.

func TXTRecordContainsKey(UInt16, UnsafeRawPointer!, UnsafePointer&lt;CChar>!) -> Int32

Allows you to determine if a given TXT Record contains a specified key.

func TXTRecordGetCount(UInt16, UnsafeRawPointer!) -> UInt16

Returns the number of keys stored in the TXT Record.

func TXTRecordGetValuePtr(UInt16, UnsafeRawPointer!, UnsafePointer&lt;CChar>!, UnsafeMutablePointer&lt;UInt8>!) -> UnsafeRawPointer!

Allows you to retrieve the value for a given key from a TXT Record.

