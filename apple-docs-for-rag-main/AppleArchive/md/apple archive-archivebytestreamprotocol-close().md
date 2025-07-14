

- Apple Archive
- ArchiveByteStreamProtocol
-  close() 

Instance Method

# close()

Closes the stream and releases associated resources.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
func close() throws
```

**Required**

## Discussion

After calling close(), expect that subsequent function calls on the stream to trigger a runtime error.

You must close all opened streams, otherwise deinitialization causes a runtime error.

## See Also

### Using Archive Byte Streams

func seek(toOffset: Int64, relativeTo: FileDescriptor.SeekOrigin) throws -> Int64

Updates the internal stream position to the specified offset relative to the specified origin.

**Required**

func cancel()

Cancels stream operations.

**Required**

