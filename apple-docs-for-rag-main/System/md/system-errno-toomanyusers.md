

- System
- Errno
-  tooManyUsers 

Type Property

# tooManyUsers

Too many users.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var tooManyUsers: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

The quota system ran out of table entries.

The corresponding C error is `EUSERS`.

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

static var notRecoverable: Errno

State not recoverable.

static var outputQueueFull: Errno

Interface output queue is full.

static var tooManyReferences: Errno

Too many references: can’t splice.

