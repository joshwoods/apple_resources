

- Foundation
- NSMutableData
-  setData(\_:) 

Instance Method

# setData(\_:)

Replaces the entire contents of the receiver with the contents of another data object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setData(_ data: Data)
```

## Parameters 

`data`  

The data object whose content replaces that of the receiver.

## Discussion

As part of its implementation, this method calls replaceBytes(in:withBytes:).

## See Also

### Modifying Bytes

func replaceBytes(in: NSRange, withBytes: UnsafeRawPointer)

Replaces with a given set of bytes a given range within the contents of the receiver.

func replaceBytes(in: NSRange, withBytes: UnsafeRawPointer?, length: Int)

Replaces with a given set of bytes a given range within the contents of the receiver.

func resetBytes(in: NSRange)

Replaces with zeroes the contents of the receiver in a given range.

