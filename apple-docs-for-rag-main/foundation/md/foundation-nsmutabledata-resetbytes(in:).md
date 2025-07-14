

- Foundation
- NSMutableData
-  resetBytes(in:) 

Instance Method

# resetBytes(in:)

Replaces with zeroes the contents of the receiver in a given range.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func resetBytes(in range: NSRange)
```

## Parameters 

`range`  

The range within the contents of the receiver to be replaced by zeros. The range must not exceed the bounds of the receiver.

## Discussion

If the location of `range` isn’t within the receiver’s range of bytes, an `NSRangeException` is raised. The receiver is resized to accommodate the new bytes, if necessary.

## See Also

### Modifying Bytes

func replaceBytes(in: NSRange, withBytes: UnsafeRawPointer)

Replaces with a given set of bytes a given range within the contents of the receiver.

func replaceBytes(in: NSRange, withBytes: UnsafeRawPointer?, length: Int)

Replaces with a given set of bytes a given range within the contents of the receiver.

func setData(Data)

Replaces the entire contents of the receiver with the contents of another data object.

