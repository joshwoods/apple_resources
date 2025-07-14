

- Metal
-  MTLBlitPassSampleBufferAttachmentDescriptorArray 

Class

# MTLBlitPassSampleBufferAttachmentDescriptorArray

A container that stores an array of sample buffer attachments for a blit pass.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class MTLBlitPassSampleBufferAttachmentDescriptorArray
```

## Overview

The number of elements in the array is at least the number of elements in an MTLDevice instance’s counterSets property.

## Topics

### Accessing a Sample Buffer Attachment Descriptor

subscript(Int) -> MTLBlitPassSampleBufferAttachmentDescriptor!

Accesses one of the array’s blit pass sample buffer attachment descriptor instances.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Configuring a Blit Command Encoder

class MTLBlitPassDescriptor

A configuration you create to customize a blit command encoder, which affects the runtime behavior of the blit pass you encode with it.

class MTLBlitPassSampleBufferAttachmentDescriptor

A configuration that instructs the GPU where to store counter data from the beginning and end of a blit pass.

