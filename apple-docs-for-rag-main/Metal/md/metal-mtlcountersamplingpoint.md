

- Metal
-  MTLCounterSamplingPoint 

Enumeration

# MTLCounterSamplingPoint

Options for different times when you can sample GPU counters.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
enum MTLCounterSamplingPoint
```

## Mentioned in 

Sampling GPU Data into Counter Sample Buffers

## Topics

### Reading Sampling Boundary Types

case atBlitBoundary

Counter sampling is allowed between blit commands in a blit pass.

case atDispatchBoundary

Counter sampling is allowed between kernel dispatches in a compute pass.

case atDrawBoundary

Counter sampling is allowed between draw commands in a render pass.

case atStageBoundary

Counter sampling is allowed at the start and end of a render pass’s vertex and fragment stages, and at the start and end of compute and blit passes.

case atTileDispatchBoundary

Counter sampling is allowed between tile dispatches in a render pass.

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

### Sampling a GPU Device’s Counters

var counterSets: [any MTLCounterSet]?

The counter sets supported by the device object.

**Required**

func supportsCounterSampling(MTLCounterSamplingPoint) -> Bool

Returns a Boolean value that indicates whether you can read GPU counters at the specified command boundary.

**Required**

func makeCounterSampleBuffer(descriptor: MTLCounterSampleBufferDescriptor) throws -> any MTLCounterSampleBuffer

Creates a counter sample buffer.

**Required**

