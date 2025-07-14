

- Apple Archive
- ArchiveStreamProtocol
-  readHeader() 

Instance Method

# readHeader()

Reads the next entry header.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
func readHeader() throws -> ArchiveHeader?
```

**Required**

## Return Value

A new header instance, or `nil` if the operation reaches the end of the archive stream.

## See Also

### Reading and Writing Headers

func writeHeader(ArchiveHeader) throws

Writes an entry header.

**Required**

