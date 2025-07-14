

- MediaExtension
- MEByteSource
-  byteSourceForRelatedFileName(\_:) 

Instance Method

# byteSourceForRelatedFileName(\_:)

Creates a new byte source for a related file.

macOS 14.0+

``` source
func byteSourceForRelatedFileName(_ fileName: String) throws -> MEByteSource
```

## Parameters 

`fileName`  

The related file name that exists in the byte source’s parent directory.

## Return Value

A byte source.

## Discussion

Requests creation of a new MEByteSource for a file related to the receiving MEByteSource. Only file names returned by the relatedFileNamesInSameDirectory method may be accessed.

## See Also

### Performing operations on a byte source

func availableLength(at: Int64) -> Int64

Gets the number of available bytes from the offset within the byte source.

func read(length: Int, from: Int64, completionHandler: (Data?, (any Error)?) -> Void)

Reads bytes from a byte source into a data object.

