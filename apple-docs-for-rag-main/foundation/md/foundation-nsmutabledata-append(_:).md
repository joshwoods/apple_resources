

- Foundation
- NSMutableData
-  append(\_:) 

Instance Method

# append(\_:)

Appends the content of another data object to the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func append(_ other: Data)
```

## Parameters 

`other`  

The data object whose content is to be appended to the contents of the receiver.

## See Also

### Adding Bytes

func append(UnsafeRawPointer, length: Int)

Appends to the receiver a given number of bytes from a given buffer.

func increaseLength(by: Int)

Increases the length of the receiver by a given number of bytes.

