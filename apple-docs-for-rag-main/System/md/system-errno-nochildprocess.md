

- System
- Errno
-  noChildProcess 

Type Property

# noChildProcess

No child processes.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var noChildProcess: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

A `wait(2)` or `waitpid(2)` function was executed by a process that dosn’t have any existing child processes or whose child processes are all already being waited for.

The corresponding C error is `ECHILD`.

## See Also

### Process Errors

static var argListTooLong: Errno

The argument list is too long.

static var identifierRemoved: Errno

Identifier removed.

static var noSuchProcess: Errno

No such process.

static var previousOwnerDied: Errno

Previous pthread mutex owner died.

static var tooManyProcesses: Errno

Too many processes.

