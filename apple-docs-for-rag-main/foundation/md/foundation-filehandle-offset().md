

- Foundation
- FileHandle
-  offset() 

Instance Method

# offset()

Gets the position of the file pointer within the file.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15.4+tvOS 13.4+visionOS 1.0+watchOS 6.2+

``` source
func offset() throws -> UInt64
```

## Return Value

The position of the file pointer within the file.

## Discussion

Throws an error if called on a file handle representing a pipe or socket, or if the file descriptor is closed.

## See Also

### Seeking Within a File

func seekToEnd() throws -> UInt64

Places the file pointer at the end of the file referenced by the file handle and returns the new file offset.

func seek(toOffset: UInt64) throws

Moves the file pointer to the specified offset within the file.

