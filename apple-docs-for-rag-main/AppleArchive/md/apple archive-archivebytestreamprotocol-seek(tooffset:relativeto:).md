

- Apple Archive
- ArchiveByteStreamProtocol
-  seek(toOffset:relativeTo:) 

Instance Method

# seek(toOffset:relativeTo:)

Updates the internal stream position to the specified offset relative to the specified origin.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
func seek(
    toOffset offset: Int64,
    relativeTo origin: FileDescriptor.SeekOrigin
) throws -> Int64
```

**Required**

## Parameters 

`offset`  

The offset relative to the reference position from which to seek.

`origin`  

The reference position from which to seek.

## Return Value

The new internal stream position that is relative to the beginning of the stream.

## See Also

### Using Archive Byte Streams

func cancel()

Cancels stream operations.

**Required**

func close() throws

Closes the stream and releases associated resources.

**Required**

