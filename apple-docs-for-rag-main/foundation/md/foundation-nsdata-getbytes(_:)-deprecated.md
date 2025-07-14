

- Foundation
- NSData
-  getBytes(\_:) Deprecated

Instance Method

# getBytes(\_:)

Copies a data object’s contents into a given buffer.

iOS 2.0–8.0DeprecatediPadOS 2.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.10DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func getBytes(_ buffer: UnsafeMutableRawPointer)
```

Deprecated

This method is unsafe because it could potentially cause buffer overruns. Use getBytes(_:length:) or getBytes(_:range:) instead.

## Parameters 

`buffer`  

A buffer into which to copy the receiver’s data. The buffer must be at least length bytes.

## Discussion

You can see a sample using this method in Working With Binary Data.

## See Also

### Related Documentation

var description: String

### Accessing Underlying Bytes

var bytes: UnsafeRawPointer

A pointer to the data object’s contents.

func enumerateBytes((UnsafeRawPointer, NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates each range of bytes in the data object using a block.

func getBytes(UnsafeMutableRawPointer, length: Int)

Copies a number of bytes from the start of the data object into a given buffer.

func getBytes(UnsafeMutableRawPointer, range: NSRange)

Copies a range of bytes from the data object into a given buffer.

