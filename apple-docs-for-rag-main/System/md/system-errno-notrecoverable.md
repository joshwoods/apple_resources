

- System
- Errno
-  notRecoverable 

Type Property

# notRecoverable

State not recoverable.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var notRecoverable: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

The corresponding C error is `ENOTRECOVERABLE`.

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

static var notPermitted: Errno

Operation not permitted.

static var outputQueueFull: Errno

Interface output queue is full.

static var tooManyReferences: Errno

Too many references: can’t splice.

static var tooManyUsers: Errno

Too many users.

