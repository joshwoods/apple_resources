

- System
- Errno
-  alreadyInProcess 

Type Property

# alreadyInProcess

Operation already in progress.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var alreadyInProcess: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

You attempted an operation on a nonblocking object that already had an operation in progress.

The corresponding C error is `EALREADY`.

## See Also

### System Call Errors

static var badAddress: Errno

Bad address.

static var interrupted: Errno

Interrupted function call.

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

