

- Foundation
- NSData
-  bytes 

Instance Property

# bytes

A pointer to the data object’s contents.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var bytes: UnsafeRawPointer { get }
```

## Discussion

If the length of the NSData object is 0, this property returns `nil`.

For an immutable data object, the returned pointer is valid until the data object is deallocated. For a mutable data object, the returned pointer is valid until the data object is deallocated or the data is mutated.

## See Also

### Related Documentation

var description: String

### Accessing Underlying Bytes

func enumerateBytes((UnsafeRawPointer, NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates each range of bytes in the data object using a block.

func getBytes(UnsafeMutableRawPointer)

Copies a data object’s contents into a given buffer.

Deprecated

func getBytes(UnsafeMutableRawPointer, length: Int)

Copies a number of bytes from the start of the data object into a given buffer.

func getBytes(UnsafeMutableRawPointer, range: NSRange)

Copies a range of bytes from the data object into a given buffer.

