

- Foundation
- NSMutableData
-  append(\_:length:) 

Instance Method

# append(\_:length:)

Appends to the receiver a given number of bytes from a given buffer.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func append(
    _ bytes: UnsafeRawPointer,
    length: Int
)
```

## Parameters 

`bytes`  

A buffer containing data to append to the receiver’s content.

`length`  

The number of bytes from `bytes` to append.

## Discussion

A sample using this method can be found in Working With Mutable Binary Data.

## See Also

### Adding Bytes

func append(Data)

Appends the content of another data object to the receiver.

func increaseLength(by: Int)

Increases the length of the receiver by a given number of bytes.

