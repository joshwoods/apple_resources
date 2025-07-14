

- System
- FileDescriptor
- FileDescriptor.SeekOrigin
-  end 

Type Property

# end

Indicates that the offset should be set to the size of the file plus the specified number of bytes.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var end: FileDescriptor.SeekOrigin { get }
```

## Mentioned in 

Adopting Swift File Options

## Discussion

The corresponding C constant is `SEEK_END`.

## See Also

### Creating a Seek Origin

static var current: FileDescriptor.SeekOrigin

Indicates that the offset should be set to the specified number of bytes after the current location.

static var nextHole: FileDescriptor.SeekOrigin

Indicates that the offset should be set to the next hole after the specified number of bytes.

static var nextData: FileDescriptor.SeekOrigin

Indicates that the offset should be set to the start of the next file region that isn’t a hole and is greater than or equal to the supplied offset.

static var start: FileDescriptor.SeekOrigin

Indicates that the offset should be set to the specified value.

