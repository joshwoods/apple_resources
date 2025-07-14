

- System
- Errno
-  invalidArgument 

Type Property

# invalidArgument

Invalid argument.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var invalidArgument: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

One or more of the specified arguments wasn’t valid; for example, specifying an undefined signal to a signal or kill function.

The corresponding C error is `EINVAL`.

## See Also

### System Call Errors

static var alreadyInProcess: Errno

Operation already in progress.

static var badAddress: Errno

Bad address.

static var interrupted: Errno

Interrupted function call.

static var noFunction: Errno

Function not implemented.

static var nowInProgress: Errno

Operation now in progress.

static var resourceBusy: Errno

Resource busy.

static var resourceTemporarilyUnavailable: Errno

Resource temporarily unavailable.

