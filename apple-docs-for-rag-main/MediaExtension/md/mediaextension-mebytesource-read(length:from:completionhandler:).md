

- MediaExtension
- MEByteSource
-  read(length:from:completionHandler:) 

Instance Method

# read(length:from:completionHandler:)

Reads bytes from a byte source into a data object.

macOS 14.0+

``` source
func read(
    length: Int,
    from offset: Int64,
    completionHandler: @escaping (Data?, (any Error)?) -> Void
)
```

``` source
func read(
    length: Int,
    from offset: Int64
) async throws -> Data
```

## Parameters 

`length`  

The number of bytes to read.

`offset`  

The relative offset in bytes from the beginning of the file from which to start reading.

`completionHandler`  

The completion block to execute when the read operation finishes.

## See Also

### Performing operations on a byte source

func availableLength(at: Int64) -> Int64

Gets the number of available bytes from the offset within the byte source.

func byteSourceForRelatedFileName(String) throws -> MEByteSource

Creates a new byte source for a related file.

