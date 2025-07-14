

- System
- Errno
-  badCPUType 

Type Property

# badCPUType

Bad CPU type in executable.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var badCPUType: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

The specified executable doesn’t support the current CPU.

The corresponding C error is `EBADARCH`.

## See Also

### Executable File Errors

static var badExecutable: Errno

Bad executable or shared library.

static var execFormatError: Errno

Executable format error.

static var malformedMachO: Errno

Malformed Mach-O file.

static var sharedLibraryVersionMismatch: Errno

Shared library version mismatch.

