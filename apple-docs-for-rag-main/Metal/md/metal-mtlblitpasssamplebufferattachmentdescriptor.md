

- Metal
-  MTLBlitPassSampleBufferAttachmentDescriptor 

Class

# MTLBlitPassSampleBufferAttachmentDescriptor

A configuration that instructs the GPU where to store counter data from the beginning and end of a blit pass.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class MTLBlitPassSampleBufferAttachmentDescriptor
```

## Mentioned in 

Sampling GPU Data into Counter Sample Buffers

## Overview

See Sampling GPU Data into Counter Sample Buffers for more context about configuring instances of this type. That article is one of a series of articles in GPU Counters and Counter Sample Buffers.

## Topics

### Configuring the Sample Buffer Attachment

var sampleBuffer: (any MTLCounterSampleBuffer)?

A specialized memory buffer that the GPU uses to store its counter data during the blit pass.

var startOfEncoderSampleIndex: Int

An index within a counter sample buffer that tells the GPU where to store counter data from the start of a blit pass.

var endOfEncoderSampleIndex: Int

An index within a counter sample buffer that tells the GPU where to store counter data from the end of a blit pass.

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

### Configuring a Blit Command Encoder

class MTLBlitPassDescriptor

A configuration you create to customize a blit command encoder, which affects the runtime behavior of the blit pass you encode with it.

class MTLBlitPassSampleBufferAttachmentDescriptorArray

A container that stores an array of sample buffer attachments for a blit pass.

