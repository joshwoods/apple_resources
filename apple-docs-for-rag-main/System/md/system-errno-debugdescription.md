

- System
- Errno
-  debugDescription 

Instance Property

# debugDescription

A textual representation, suitable for debugging, of the most recent error returned by a system call.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var debugDescription: String { get }
```

## Discussion

The corresponding C function is `strerror(3)`.

## See Also

### Debugging

var description: String

A textual representation of the most recent error returned by a system call.

