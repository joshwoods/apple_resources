

- System
- Errno
-  noMemory 

Type Property

# noMemory

Can’t allocate memory.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var noMemory: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

The new process image required more memory than was allowed by the hardware or by system-imposed memory management constraints. A lack of swap space is normally temporary; however, a lack of core is not. You can increase soft limits up to their corresponding hard limits.

The corresponding C error is `ENOMEM`.

## See Also

### Runtime Errors

static var deadlock: Errno

Resource deadlock avoided.

static var wouldBlock: Errno

Operation would block.

