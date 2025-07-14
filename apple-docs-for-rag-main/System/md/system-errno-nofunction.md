

- System
- Errno
-  noFunction 

Type Property

# noFunction

Function not implemented.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var noFunction: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

You attempted a system call that isn’t available on this system.

The corresponding C error is `ENOSYS`.

## See Also

### System Call Errors

static var alreadyInProcess: Errno

Operation already in progress.

static var badAddress: Errno

Bad address.

static var interrupted: Errno

Interrupted function call.

static var invalidArgument: Errno

Invalid argument.

static var nowInProgress: Errno

Operation now in progress.

static var resourceBusy: Errno

Resource busy.

static var resourceTemporarilyUnavailable: Errno

Resource temporarily unavailable.

