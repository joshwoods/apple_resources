

- Metal
-  MTLBlitPassDescriptor 

Class

# MTLBlitPassDescriptor

A configuration you create to customize a blit command encoder, which affects the runtime behavior of the blit pass you encode with it.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class MTLBlitPassDescriptor
```

## Mentioned in 

Sampling GPU Data into Counter Sample Buffers

## Overview

You can customize an encoder for a blit pass by creating and configuring an MTLBlitPassDescriptor instance and passing it to makeBlitCommandEncoder(descriptor:).

## Topics

### Configuring Sample Buffer Attachment Descriptors for a Blit Pass

var sampleBufferAttachments: MTLBlitPassSampleBufferAttachmentDescriptorArray

An array of counter sample buffer attachments that you configure for a blit pass.

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

class MTLBlitPassSampleBufferAttachmentDescriptor

A configuration that instructs the GPU where to store counter data from the beginning and end of a blit pass.

class MTLBlitPassSampleBufferAttachmentDescriptorArray

A container that stores an array of sample buffer attachments for a blit pass.

