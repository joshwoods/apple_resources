

- System
- Errno
-  badAddress 

Type Property

# badAddress

Bad address.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var badAddress: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

An address passed as an argument to a system call was invalid.

The corresponding C error is `EFAULT`.

## See Also

### System Call Errors

static var alreadyInProcess: Errno

Operation already in progress.

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

