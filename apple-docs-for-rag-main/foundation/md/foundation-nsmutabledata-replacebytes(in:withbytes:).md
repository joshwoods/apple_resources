

- Foundation
- NSMutableData
-  replaceBytes(in:withBytes:) 

Instance Method

# replaceBytes(in:withBytes:)

Replaces with a given set of bytes a given range within the contents of the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func replaceBytes(
    in range: NSRange,
    withBytes bytes: UnsafeRawPointer
)
```

## Parameters 

`range`  

The range within the receiver’s contents to replace with `bytes`. The range must not exceed the bounds of the receiver.

`bytes`  

The data to insert into the receiver’s contents.

## Discussion

If the location of `range` isn’t within the receiver’s range of bytes, an `NSRangeException` is raised. The receiver is resized to accommodate the new bytes, if necessary.

A sample using this method is given in Working With Mutable Binary Data.

## See Also

### Modifying Bytes

func replaceBytes(in: NSRange, withBytes: UnsafeRawPointer?, length: Int)

Replaces with a given set of bytes a given range within the contents of the receiver.

func resetBytes(in: NSRange)

Replaces with zeroes the contents of the receiver in a given range.

func setData(Data)

Replaces the entire contents of the receiver with the contents of another data object.

