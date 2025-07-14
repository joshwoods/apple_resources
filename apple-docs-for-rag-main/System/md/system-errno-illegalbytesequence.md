

- System
- Errno
-  illegalByteSequence 

Type Property

# illegalByteSequence

Illegal byte sequence.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var illegalByteSequence: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

While decoding a multibyte character, the function encountered an invalid or incomplete sequence of bytes, or the given wide character is invalid.

The corresponding C error is `EILSEQ`.

## See Also

### General Errors

static var badMessage: Errno

Bad message.

static var canceled: Errno

Operation canceled.

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

static var tooManyUsers: Errno

Too many users.

