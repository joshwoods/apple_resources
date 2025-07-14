

- Core Video
-  CVPlanarComponentInfo 

Structure

# CVPlanarComponentInfo

A structure for describing planar components.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
struct CVPlanarComponentInfo
```

## Overview

Depending on how they were created, planar pixel buffers may or may not have this descriptor at their base address. For this reason, you should use CVPixelBufferGetBaseAddressOfPlane(_:_:) and CVPixelBufferGetBytesPerRowOfPlane(_:_:) to get information about a planar pixel buffer.

## Topics

### Initializers

init()

init(offset: Int32, rowBytes: UInt32)

### Properties

var offset: Int32

The offset from the main base address to the base address of this plane. (big-endian)

var rowBytes: UInt32

The number of bytes per row of this plane. (big-endian)

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Data Types

typealias CVPixelBuffer

A reference to a Core Video pixel buffer object.

struct CVPixelBufferLockFlags

The flags to pass to CVPixelBufferLockBaseAddress(_:_:) and CVPixelBufferUnlockBaseAddress(_:_:).

struct CVPlanarPixelBufferInfo

A structure for describing planar buffers.

struct CVPlanarPixelBufferInfo_YCbCrPlanar

A structure for describing YCbCr planar buffers.

struct CVPlanarPixelBufferInfo_YCbCrBiPlanar

A structure for describing YCbCr biplanar buffers.

