

- Foundation
- NSData
-  enumerateBytes(\_:) 

Instance Method

# enumerateBytes(\_:)

Enumerates each range of bytes in the data object using a block.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func enumerateBytes(_ block: (UnsafeRawPointer, NSRange, UnsafeMutablePointer) -> Void)
```

## Parameters 

`block`  

The block to apply to byte ranges in the array.

The block takes three arguments:

bytes  
The bytes for the current range. This pointer is valid until the data object is deallocated.

byteRange  
The range of the current data bytes.

stop  
A reference to a Boolean value. The block can set the value to true to stop further processing of the data. The stop argument is an out-only argument. You should only ever set this Boolean to true within the Block.

## Discussion

The enumeration block is called once for each contiguous region of memory in the receiver (once total for a contiguous NSData object), until either all bytes have been enumerated, or the `stop` parameter is set to true.

## See Also

### Accessing Underlying Bytes

var bytes: UnsafeRawPointer

A pointer to the data object’s contents.

func getBytes(UnsafeMutableRawPointer)

Copies a data object’s contents into a given buffer.

Deprecated

func getBytes(UnsafeMutableRawPointer, length: Int)

Copies a number of bytes from the start of the data object into a given buffer.

func getBytes(UnsafeMutableRawPointer, range: NSRange)

Copies a range of bytes from the data object into a given buffer.

