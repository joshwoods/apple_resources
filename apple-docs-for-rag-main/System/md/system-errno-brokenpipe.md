

- System
- Errno
-  brokenPipe 

Type Property

# brokenPipe

Broken pipe.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var brokenPipe: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

You attempted to write to a pipe, socket, or FIFO that doesn’t have a process reading its data.

The corresponding C error is `EPIPE`.

## See Also

### Pipe Errors

static var illegalSeek: Errno

Illegal seek.

