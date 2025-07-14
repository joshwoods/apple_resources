

- Foundation
- NSData
-  getBytes(\_:length:) 

Instance Method

# getBytes(\_:length:)

Copies a number of bytes from the start of the data object into a given buffer.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func getBytes(
    _ buffer: UnsafeMutableRawPointer,
    length: Int
)
```

## Parameters 

`buffer`  

A buffer into which to copy data.

`length`  

The number of bytes from the start of the receiver’s data to copy to `buffer`.

## Discussion

The number of bytes copied is the smaller of the `length` parameter and the length of the data encapsulated in the object.

## See Also

### Related Documentation

var description: String

### Accessing Underlying Bytes

var bytes: UnsafeRawPointer

A pointer to the data object’s contents.

func enumerateBytes((UnsafeRawPointer, NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates each range of bytes in the data object using a block.

func getBytes(UnsafeMutableRawPointer)

Copies a data object’s contents into a given buffer.

Deprecated

func getBytes(UnsafeMutableRawPointer, range: NSRange)

Copies a range of bytes from the data object into a given buffer.

