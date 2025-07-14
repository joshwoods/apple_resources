

- System
- Errno
-  execFormatError 

Type Property

# execFormatError

Executable format error.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var execFormatError: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

A request was made to execute a file that, although it has the appropriate permissions, isn’t in the format required for an executable file.

The corresponding C error is `ENOEXEC`.

## See Also

### Executable File Errors

static var badCPUType: Errno

Bad CPU type in executable.

static var badExecutable: Errno

Bad executable or shared library.

static var malformedMachO: Errno

Malformed Mach-O file.

static var sharedLibraryVersionMismatch: Errno

Shared library version mismatch.

