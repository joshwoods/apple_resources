

- Apple Archive
- ArchiveByteStreamProtocol
-  cancel() 

Instance Method

# cancel()

Cancels stream operations.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
func cancel()
```

**Required**

## Discussion

Note that after you’ve called cancel(), you must close the stream to release resources.

## See Also

### Using Archive Byte Streams

func seek(toOffset: Int64, relativeTo: FileDescriptor.SeekOrigin) throws -> Int64

Updates the internal stream position to the specified offset relative to the specified origin.

**Required**

func close() throws

Closes the stream and releases associated resources.

**Required**

