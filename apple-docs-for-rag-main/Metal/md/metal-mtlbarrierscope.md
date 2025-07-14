

- Metal
-  MTLBarrierScope 

Structure

# MTLBarrierScope

Describes the types of resources that a barrier operates on.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
struct MTLBarrierScope
```

## Topics

### Initializers

init(rawValue: UInt)

### Type Properties

static var buffers: MTLBarrierScope

The barrier affects any buffer objects.

static var renderTargets: MTLBarrierScope

The barrier affects any render targets.

static var textures: MTLBarrierScope

The barrier affects textures.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Memory Barriers and Fences

Implementing a Multistage Image Filter Using Heaps and Fences

Use fences to synchronize access to resources allocated on a heap.

protocol MTLFence

A memory fence to capture, track, and manage resource dependencies across command encoders.

