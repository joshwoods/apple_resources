

- dnssd
-  TXTRecordGetCount(\_:\_:) 

Function

# TXTRecordGetCount(\_:\_:)

Returns the number of keys stored in the TXT Record.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func TXTRecordGetCount(
    _ txtLen: UInt16,
    _ txtRecord: UnsafeRawPointer!
) -> UInt16
```

## Parameters 

`txtLen`  

The size of the received TXT Record.

`txtRecord`  

Pointer to the received TXT Record bytes.

## Return Value

Returns the total number of keys in the TXT Record.

## Discussion

The count can be used with TXTRecordGetItemAtIndex() to iterate through the keys.

## See Also

### TXT Record Parsing Functions

DNSServiceCreateDelegateConnection

Create a delegate connection to the daemon allowing efficient registration of multiple individual records.

func DNSServiceSetDispatchQueue(DNSServiceRef!, dispatch_queue_t!) -> DNSServiceErrorType

Allows you to schedule a DNSServiceRef on a serial dispatch queue for receiving asynchronous callbacks.

func TXTRecordContainsKey(UInt16, UnsafeRawPointer!, UnsafePointer&lt;CChar>!) -> Int32

Allows you to determine if a given TXT Record contains a specified key.

func TXTRecordGetItemAtIndex(UInt16, UnsafeRawPointer!, UInt16, UInt16, UnsafeMutablePointer&lt;CChar>!, UnsafeMutablePointer&lt;UInt8>!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!) -> DNSServiceErrorType

Allows you to retrieve a key name and value pointer, given an index into a TXT Record.

func TXTRecordGetValuePtr(UInt16, UnsafeRawPointer!, UnsafePointer&lt;CChar>!, UnsafeMutablePointer&lt;UInt8>!) -> UnsafeRawPointer!

Allows you to retrieve the value for a given key from a TXT Record.

