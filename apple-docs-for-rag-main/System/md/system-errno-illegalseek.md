

- System
- Errno
-  illegalSeek 

Type Property

# illegalSeek

Illegal seek.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var illegalSeek: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

An `lseek(2)` function was issued on a socket, pipe or FIFO.

The corresponding C error is `ESPIPE`.

## See Also

### Pipe Errors

static var brokenPipe: Errno

Broken pipe.

