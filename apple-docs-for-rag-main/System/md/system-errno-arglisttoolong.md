

- System
- Errno
-  argListTooLong 

Type Property

# argListTooLong

The argument list is too long.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var argListTooLong: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

The number of bytes used for the argument and environment list of the new process exceeded the limit `NCARGS`, as defined in ``.

The corresponding C error is `E2BIG`.

## See Also

### Process Errors

static var identifierRemoved: Errno

Identifier removed.

static var noChildProcess: Errno

No child processes.

static var noSuchProcess: Errno

No such process.

static var previousOwnerDied: Errno

Previous pthread mutex owner died.

static var tooManyProcesses: Errno

Too many processes.

