

- System
- Errno
-  interrupted 

Type Property

# interrupted

Interrupted function call.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var interrupted: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

The process caught an asynchronous signal (such as `SIGINT` or `SIGQUIT`) during the execution of an interruptible function. If the signal handler performs a normal return, the caller of the interrupted function call receives this error.

The corresponding C error is `EINTR`.

## See Also

### System Call Errors

static var alreadyInProcess: Errno

Operation already in progress.

static var badAddress: Errno

Bad address.

static var invalidArgument: Errno

Invalid argument.

static var noFunction: Errno

Function not implemented.

static var nowInProgress: Errno

Operation now in progress.

static var resourceBusy: Errno

Resource busy.

static var resourceTemporarilyUnavailable: Errno

Resource temporarily unavailable.

