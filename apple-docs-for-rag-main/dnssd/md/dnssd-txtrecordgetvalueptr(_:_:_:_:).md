

- dnssd
-  TXTRecordGetValuePtr(\_:\_:\_:\_:) 

Function

# TXTRecordGetValuePtr(\_:\_:\_:\_:)

Allows you to retrieve the value for a given key from a TXT Record.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func TXTRecordGetValuePtr(
    _ txtLen: UInt16,
    _ txtRecord: UnsafeRawPointer!,
    _ key: UnsafePointer!,
    _ valueLen: UnsafeMutablePointer!
) -> UnsafeRawPointer!
```

## Parameters 

`txtLen`  

The size of the received TXT Record

`txtRecord`  

Pointer to the received TXT Record bytes.

`key`  

A null-terminated ASCII string containing the key name.

`valueLen`  

On output, will be set to the size of the “value” data.

## Return Value

Returns NULL if the key does not exist in this TXT record, or exists with no value (to differentiate between these two cases use TXTRecordContainsKey()). Returns pointer to location within TXT Record bytes if the key exists with empty or non-empty value. For empty value, valueLen will be zero. For non-empty value, valueLen will be length of value data.

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

func TXTRecordGetItemAtIndex(UInt16, UnsafeRawPointer!, UInt16, UInt16, UnsafeMutablePointer&lt;CChar>!, UnsafeMutablePointer&lt;UInt8>!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!) -> DNSServiceErrorType

Allows you to retrieve a key name and value pointer, given an index into a TXT Record.

