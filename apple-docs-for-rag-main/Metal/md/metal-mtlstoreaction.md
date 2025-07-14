

- Metal
-  MTLStoreAction 

Enumeration

# MTLStoreAction

Types of actions performed for an attachment at the end of a rendering pass.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
enum MTLStoreAction
```

## Mentioned in 

Setting Load and Store Actions

## Topics

### Constants

case dontCare

The GPU has permission to discard the rendered contents of the attachment at the end of the render pass, replacing them with arbitrary data.

case store

The GPU stores the rendered contents to the texture.

case multisampleResolve

The GPU resolves the multisampled data to one sample per pixel and stores the data to the resolve texture, discarding the multisample data afterwards.

case storeAndMultisampleResolve

The GPU stores the multisample data to the multisample texture, resolves the data to a sample per pixel, and stores the data to the resolve texture.

case unknown

The system selects a store action when it encodes the render pass.

case customSampleDepthStore

The GPU stores depth data in a sample-position–agnostic representation.

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

enum MTLLoadAction

Types of actions performed for an attachment at the start of a rendering pass.

struct MTLStoreActionOptions

Options that modify a store action.

