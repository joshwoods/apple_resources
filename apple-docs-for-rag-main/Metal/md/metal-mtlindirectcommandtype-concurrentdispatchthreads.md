

- Metal
- MTLIndirectCommandType
-  concurrentDispatchThreads 

Type Property

# concurrentDispatchThreads

A compute command using an arbitrarily sized grid.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 11.0+tvOS 13.0+visionOS 1.0+

``` source
static var concurrentDispatchThreads: MTLIndirectCommandType { get }
```

## See Also

### Specifying Command Types

static var draw: MTLIndirectCommandType

A draw call command.

static var drawIndexed: MTLIndirectCommandType

An indexed draw call command.

static var drawPatches: MTLIndirectCommandType

A draw call command for tessellated patches.

static var drawIndexedPatches: MTLIndirectCommandType

An indexed draw call command for tessellated patches.

static var concurrentDispatch: MTLIndirectCommandType

A compute command using a grid aligned to threadgroup boundaries.

