

- System
- FileDescriptor
-  seek(offset:from:) 

Instance Method

# seek(offset:from:)

Repositions the offset for the given file descriptor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@discardableResult
func seek(
    offset: Int64,
    from whence: FileDescriptor.SeekOrigin
) throws -> Int64
```

## Parameters 

`offset`  

The new offset for the file descriptor.

`whence`  

The origin of the new offset.

## Return Value

The file’s offset location, in bytes from the beginning of the file.

## Discussion

The corresponding C function is `lseek`.

## See Also

### Changing a File’s Offset

struct SeekOrigin

Options for specifying what a file descriptor’s offset is relative to.

