

- System
- Errno
-  sharedLibraryVersionMismatch 

Type Property

# sharedLibraryVersionMismatch

Shared library version mismatch.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var sharedLibraryVersionMismatch: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

The version of the shared library on the system doesn’t match the expected version.

The corresponding C error is `ESHLIBVERS`.

## See Also

### Executable File Errors

static var badCPUType: Errno

Bad CPU type in executable.

static var badExecutable: Errno

Bad executable or shared library.

static var execFormatError: Errno

Executable format error.

static var malformedMachO: Errno

Malformed Mach-O file.

