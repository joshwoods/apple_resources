

- System
- FileDescriptor
- FileDescriptor.AccessMode
-  readWrite 

Type Property

# readWrite

Opens the file for reading and writing.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var readWrite: FileDescriptor.AccessMode { get }
```

## Mentioned in 

Adopting Swift File Options

## Discussion

The corresponding C constant is `O_RDWR`.

## See Also

### Creating an Access Mode

static var readOnly: FileDescriptor.AccessMode

Opens the file for reading only.

static var writeOnly: FileDescriptor.AccessMode

Opens the file for writing only.

