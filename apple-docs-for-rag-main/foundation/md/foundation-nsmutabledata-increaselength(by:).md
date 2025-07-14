

- Foundation
- NSMutableData
-  increaseLength(by:) 

Instance Method

# increaseLength(by:)

Increases the length of the receiver by a given number of bytes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func increaseLength(by extraLength: Int)
```

## Parameters 

`extraLength`  

The number of bytes by which to increase the receiver’s length.

## Discussion

The additional bytes are all set to `0`.

Important

Changing the length of a mutable data object invalidates any existing data pointers returned by the bytes or mutableBytes properties.

## See Also

### Related Documentation

var length: Int

The number of bytes contained in the mutable data object.

### Adding Bytes

func append(UnsafeRawPointer, length: Int)

Appends to the receiver a given number of bytes from a given buffer.

func append(Data)

Appends the content of another data object to the receiver.

