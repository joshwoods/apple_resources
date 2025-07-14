

- Metal
-  MTLAccelerationStructurePassSampleBufferAttachmentDescriptor 

Class

# MTLAccelerationStructurePassSampleBufferAttachmentDescriptor

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class MTLAccelerationStructurePassSampleBufferAttachmentDescriptor
```

## Mentioned in 

Sampling GPU Data into Counter Sample Buffers

## Topics

### Instance Properties

var endOfEncoderSampleIndex: Int

var sampleBuffer: (any MTLCounterSampleBuffer)?

A specialized memory buffer that the GPU uses to store its counter data during the acceleration structure pass.

var startOfEncoderSampleIndex: Int

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Acceleration Structures Passes

class MTLAccelerationStructurePassDescriptor

class MTLAccelerationStructurePassSampleBufferAttachmentDescriptorArray

