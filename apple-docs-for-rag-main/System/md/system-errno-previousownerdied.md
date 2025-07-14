

- System
- Errno
-  previousOwnerDied 

Type Property

# previousOwnerDied

Previous pthread mutex owner died.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var previousOwnerDied: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

The corresponding C error is `EOWNERDEAD`.

## See Also

### Process Errors

static var argListTooLong: Errno

The argument list is too long.

static var identifierRemoved: Errno

Identifier removed.

static var noChildProcess: Errno

No child processes.

static var noSuchProcess: Errno

No such process.

static var tooManyProcesses: Errno

Too many processes.

