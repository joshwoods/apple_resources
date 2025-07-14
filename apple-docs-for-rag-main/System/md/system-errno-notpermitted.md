

- System
- Errno
-  notPermitted 

Type Property

# notPermitted

Operation not permitted.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var notPermitted: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

An attempt was made to perform an operation limited to processes with appropriate privileges or to the owner of a file or other resources.

The corresponding C error is `EPERM`.

## See Also

### General Errors

static var badMessage: Errno

Bad message.

static var canceled: Errno

Operation canceled.

static var illegalByteSequence: Errno

Illegal byte sequence.

static var noData: Errno

No message available.

static var noMessage: Errno

No message of desired type.

static var noSuchPolicy: Errno

No such policy registered.

static var notRecoverable: Errno

State not recoverable.

static var outputQueueFull: Errno

Interface output queue is full.

static var tooManyReferences: Errno

Too many references: can’t splice.

static var tooManyUsers: Errno

Too many users.

