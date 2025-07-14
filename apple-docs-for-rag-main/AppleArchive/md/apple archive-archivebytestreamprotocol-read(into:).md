

- Apple Archive
- ArchiveByteStreamProtocol
-  read(into:) 

Instance Method

# read(into:)

Reads data to the specified buffer, not exceeding the buffer’s previously allocated size.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
func read(into buffer: UnsafeMutableRawBufferPointer) throws -> Int
```

**Required**

## Parameters 

`buffer`  

The data buffer that the operation fills with the read bytes.

## Return Value

The number of bytes read and stored by the stream.

## Discussion

This function increments the internal stream position by the number of bytes read by the stream.

## See Also

### Reading and Writing Data

func read(into: UnsafeMutableRawBufferPointer, atOffset: Int64) throws -> Int

Reads data at the supplied offset to the specified buffer, not exceeding the buffer’s previously allocated size.

**Required**

func write(from: UnsafeRawBufferPointer) throws -> Int

Writes data from the specified buffer, not exceeding the buffer’s allocated size.

**Required**

func write(from: UnsafeRawBufferPointer, atOffset: Int64) throws -> Int

Writes data at the supplied offset from the specified buffer, not exceeding the buffer’s allocated size.

**Required**

