

- System
- Errno
-  noSuchProcess 

Type Property

# noSuchProcess

No such process.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var noSuchProcess: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

There isn’t a process that corresponds to the specified process ID.

The corresponding C error is `ESRCH`.

## See Also

### Process Errors

static var argListTooLong: Errno

The argument list is too long.

static var identifierRemoved: Errno

Identifier removed.

static var noChildProcess: Errno

No child processes.

static var previousOwnerDied: Errno

Previous pthread mutex owner died.

static var tooManyProcesses: Errno

Too many processes.

