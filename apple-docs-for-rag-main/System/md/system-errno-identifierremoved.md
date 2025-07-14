

- System
- Errno
-  identifierRemoved 

Type Property

# identifierRemoved

Identifier removed.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var identifierRemoved: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

An IPC identifier was removed while the current process was waiting on it.

The corresponding C error is `EIDRM`.

## See Also

### Process Errors

static var argListTooLong: Errno

The argument list is too long.

static var noChildProcess: Errno

No child processes.

static var noSuchProcess: Errno

No such process.

static var previousOwnerDied: Errno

Previous pthread mutex owner died.

static var tooManyProcesses: Errno

Too many processes.

