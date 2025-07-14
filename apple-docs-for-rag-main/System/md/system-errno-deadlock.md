

- System
- Errno
-  deadlock 

Type Property

# deadlock

Resource deadlock avoided.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var deadlock: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

You attempted to lock a system resource that would have resulted in a deadlock.

The corresponding C error is `EDEADLK`.

## See Also

### Runtime Errors

static var noMemory: Errno

Can’t allocate memory.

static var wouldBlock: Errno

Operation would block.

