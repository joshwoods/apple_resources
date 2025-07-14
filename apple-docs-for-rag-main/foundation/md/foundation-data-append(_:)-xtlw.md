

- Foundation
- Data
-  append(\_:) 

Instance Method

# append(\_:)

Append a buffer of bytes to the data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func append(_ buffer: UnsafeBufferPointer)
```

## Parameters 

`buffer`  

The buffer of bytes to append. The size is calculated from `SourceType` and `buffer.count`.

## See Also

### Adding Bytes

func append(Data)

Appends the specified data to the end of this data.

func append(UnsafePointer&lt;UInt8>, count: Int)

Appends the specified bytes from memory to the end of the data.

func append(contentsOf: [UInt8])

Appends the bytes in the specified array to the end of the data.

