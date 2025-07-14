

- System
- Errno
-  malformedMachO 

Type Property

# malformedMachO

Malformed Mach-O file.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var malformedMachO: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

The Mach object file is malformed.

The corresponding C error is `EBADMACHO`.

## See Also

### Executable File Errors

static var badCPUType: Errno

Bad CPU type in executable.

static var badExecutable: Errno

Bad executable or shared library.

static var execFormatError: Errno

Executable format error.

static var sharedLibraryVersionMismatch: Errno

Shared library version mismatch.

