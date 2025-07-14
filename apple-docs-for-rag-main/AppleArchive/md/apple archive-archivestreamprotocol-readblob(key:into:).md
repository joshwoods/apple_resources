

- Apple Archive
- ArchiveStreamProtocol
-  readBlob(key:into:) 

Instance Method

# readBlob(key:into:)

Reads the current entry blob data.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
func readBlob(
    key: ArchiveHeader.FieldKey,
    into buffer: UnsafeMutableRawBufferPointer
) throws
```

**Required**

## Parameters 

`key`  

The blob field key.

`buffer`  

The data buffer that the operation fills with the entry blob data.

## See Also

### Reading and Writing Blobs

func writeBlob(key: ArchiveHeader.FieldKey, from: UnsafeRawBufferPointer) throws

Writes an entry blob data.

**Required**

