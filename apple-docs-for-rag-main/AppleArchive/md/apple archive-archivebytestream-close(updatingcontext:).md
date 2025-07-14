

- Apple Archive
- ArchiveByteStream
-  close(updatingContext:) 

Instance Method

# close(updatingContext:)

Closes the stream, releases associated resources, and writes the sealed container attributes to the specified encryption context.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func close(updatingContext context: ArchiveEncryptionContext) throws
```

## Parameters 

`context`  

The encryption context that receives the sealed container attributes.

