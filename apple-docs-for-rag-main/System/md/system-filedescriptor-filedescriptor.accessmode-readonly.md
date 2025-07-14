

- System
- FileDescriptor
- FileDescriptor.AccessMode
-  readOnly 

Type Property

# readOnly

Opens the file for reading only.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var readOnly: FileDescriptor.AccessMode { get }
```

## Mentioned in 

Adopting Swift File Options

## Discussion

The corresponding C constant is `O_RDONLY`.

## See Also

### Creating an Access Mode

static var readWrite: FileDescriptor.AccessMode

Opens the file for reading and writing.

static var writeOnly: FileDescriptor.AccessMode

Opens the file for writing only.

