

- Metal
- MTLIndirectCommandType
-  draw 

Type Property

# draw

A draw call command.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
static var draw: MTLIndirectCommandType { get }
```

## See Also

### Specifying Command Types

static var drawIndexed: MTLIndirectCommandType

An indexed draw call command.

static var drawPatches: MTLIndirectCommandType

A draw call command for tessellated patches.

static var drawIndexedPatches: MTLIndirectCommandType

An indexed draw call command for tessellated patches.

static var concurrentDispatch: MTLIndirectCommandType

A compute command using a grid aligned to threadgroup boundaries.

static var concurrentDispatchThreads: MTLIndirectCommandType

A compute command using an arbitrarily sized grid.

