

- Apple Archive
- ArchiveByteStreamProtocol
-  read(into:atOffset:) 

Instance Method

# read(into:atOffset:)

Reads data at the supplied offset to the specified buffer, not exceeding the buffer’s previously allocated size.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
func read(
    into buffer: UnsafeMutableRawBufferPointer,
    atOffset offset: Int64
) throws -> Int
```

**Required**

## Parameters 

`buffer`  

The data buffer that the operation fills with the read bytes.

`offset`  

The stream position of the segment that the operation reads.

## Return Value

The number of bytes read by the stream.

## See Also

### Reading and Writing Data

func read(into: UnsafeMutableRawBufferPointer) throws -> Int

Reads data to the specified buffer, not exceeding the buffer’s previously allocated size.

**Required**

func write(from: UnsafeRawBufferPointer) throws -> Int

Writes data from the specified buffer, not exceeding the buffer’s allocated size.

**Required**

func write(from: UnsafeRawBufferPointer, atOffset: Int64) throws -> Int

Writes data at the supplied offset from the specified buffer, not exceeding the buffer’s allocated size.

**Required**

