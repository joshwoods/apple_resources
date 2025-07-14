

- dnssd
-  TXTRecordContainsKey(\_:\_:\_:) 

Function

# TXTRecordContainsKey(\_:\_:\_:)

Allows you to determine if a given TXT Record contains a specified key.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func TXTRecordContainsKey(
    _ txtLen: UInt16,
    _ txtRecord: UnsafeRawPointer!,
    _ key: UnsafePointer!
) -> Int32
```

## Parameters 

`txtLen`  

The size of the received TXT Record.

`txtRecord`  

Pointer to the received TXT Record bytes.

`key`  

A null-terminated ASCII string containing the key name.

## Return Value

Returns 1 if the TXT Record contains the specified key. Otherwise, it returns 0.

## See Also

### TXT Record Parsing Functions

DNSServiceCreateDelegateConnection

Create a delegate connection to the daemon allowing efficient registration of multiple individual records.

func DNSServiceSetDispatchQueue(DNSServiceRef!, dispatch_queue_t!) -> DNSServiceErrorType

Allows you to schedule a DNSServiceRef on a serial dispatch queue for receiving asynchronous callbacks.

func TXTRecordGetCount(UInt16, UnsafeRawPointer!) -> UInt16

Returns the number of keys stored in the TXT Record.

func TXTRecordGetItemAtIndex(UInt16, UnsafeRawPointer!, UInt16, UInt16, UnsafeMutablePointer&lt;CChar>!, UnsafeMutablePointer&lt;UInt8>!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!) -> DNSServiceErrorType

Allows you to retrieve a key name and value pointer, given an index into a TXT Record.

func TXTRecordGetValuePtr(UInt16, UnsafeRawPointer!, UnsafePointer&lt;CChar>!, UnsafeMutablePointer&lt;UInt8>!) -> UnsafeRawPointer!

Allows you to retrieve the value for a given key from a TXT Record.

