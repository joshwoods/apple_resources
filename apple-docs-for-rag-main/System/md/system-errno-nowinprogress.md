

- System
- Errno
-  nowInProgress 

Type Property

# nowInProgress

Operation now in progress.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var nowInProgress: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

You attempted an operation that takes a long time to complete, such as `connect(2)` or `connectx(2)`, on a nonblocking object. See also `fcntl(2)`.

The corresponding C error is `EINPROGRESS`.

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

static var noFunction: Errno

Function not implemented.

static var resourceBusy: Errno

Resource busy.

static var resourceTemporarilyUnavailable: Errno

Resource temporarily unavailable.

