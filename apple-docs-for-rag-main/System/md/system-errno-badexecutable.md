

- System
- Errno
-  badExecutable 

Type Property

# badExecutable

Bad executable or shared library.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var badExecutable: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

The executable or shared library being referenced was malformed.

The corresponding C error is `EBADEXEC`.

## See Also

### Executable File Errors

static var badCPUType: Errno

Bad CPU type in executable.

static var execFormatError: Errno

Executable format error.

static var malformedMachO: Errno

Malformed Mach-O file.

static var sharedLibraryVersionMismatch: Errno

Shared library version mismatch.

