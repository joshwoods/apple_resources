

- Apple Archive
- ArchiveStreamProtocol
-  writeBlob(key:from:) 

Instance Method

# writeBlob(key:from:)

Writes an entry blob data.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
func writeBlob(
    key: ArchiveHeader.FieldKey,
    from buffer: UnsafeRawBufferPointer
) throws
```

**Required**

## Parameters 

`key`  

The blob field key.

`buffer`  

The data buffer that the operation uses as a source for the entry blob data.

## See Also

### Reading and Writing Blobs

func readBlob(key: ArchiveHeader.FieldKey, into: UnsafeMutableRawBufferPointer) throws

Reads the current entry blob data.

**Required**

