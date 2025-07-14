

- System
- Errno
-  resourceBusy 

Type Property

# resourceBusy

Resource busy.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var resourceBusy: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

You attempted to use a system resource which was in use at the time, in a manner that would have conflicted with the request.

The corresponding C error is `EBUSY`.

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

static var resourceTemporarilyUnavailable: Errno

Resource temporarily unavailable.

