

- Metal
-  MTLLoadAction 

Enumeration

# MTLLoadAction

Types of actions performed for an attachment at the start of a rendering pass.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
enum MTLLoadAction
```

## Mentioned in 

Setting Load and Store Actions

## Topics

### Constants

case dontCare

The GPU has permission to discard the existing contents of the attachment at the start of the render pass, replacing them with arbitrary data.

case load

The GPU preserves the existing contents of the attachment at the start of the render pass.

case clear

The GPU writes a value to every pixel in the attachment at the start of the render pass.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Encoding a Render Pass in Parallel

protocol MTLParallelRenderCommandEncoder

An object that splits up a single render pass so that it can be simultaneously encoded from multiple threads.

enum MTLStoreAction

Types of actions performed for an attachment at the end of a rendering pass.

struct MTLStoreActionOptions

Options that modify a store action.

