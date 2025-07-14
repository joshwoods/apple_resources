

- MediaExtension
- MEByteSource
-  availableLength(at:) 

Instance Method

# availableLength(at:)

Gets the number of available bytes from the offset within the byte source.

macOS 14.0+

``` source
func availableLength(at offset: Int64) -> Int64
```

## Parameters 

`offset`  

The offset in bytes from the beginning of the byte source.

## Return Value

An integer that specifies the number of available bytes.

## See Also

### Performing operations on a byte source

func byteSourceForRelatedFileName(String) throws -> MEByteSource

Creates a new byte source for a related file.

func read(length: Int, from: Int64, completionHandler: (Data?, (any Error)?) -> Void)

Reads bytes from a byte source into a data object.

