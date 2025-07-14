

- Apple Archive
- ArchiveStreamProtocol
-  writeHeader(\_:) 

Instance Method

# writeHeader(\_:)

Writes an entry header.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
func writeHeader(_ header: ArchiveHeader) throws
```

**Required**

## Parameters 

`header`  

The entry header to which the operation writes.

## See Also

### Reading and Writing Headers

func readHeader() throws -> ArchiveHeader?

Reads the next entry header.

**Required**

