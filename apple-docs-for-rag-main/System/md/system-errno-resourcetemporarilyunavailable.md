

- System
- Errno
-  resourceTemporarilyUnavailable 

Type Property

# resourceTemporarilyUnavailable

Resource temporarily unavailable.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var resourceTemporarilyUnavailable: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

This is a temporary condition; later calls to the same routine may complete normally. Make the same function call again later.

The corresponding C error is `EAGAIN`.

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

static var nowInProgress: Errno

Operation now in progress.

static var resourceBusy: Errno

Resource busy.

