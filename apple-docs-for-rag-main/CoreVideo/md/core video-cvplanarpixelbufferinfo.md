

- Core Video
-  CVPlanarPixelBufferInfo 

Structure

# CVPlanarPixelBufferInfo

A structure for describing planar buffers.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
struct CVPlanarPixelBufferInfo
```

## Topics

### Initializers

init()

init(componentInfo: CVPlanarComponentInfo)

### Properties

var componentInfo: CVPlanarComponentInfo

An array containing a CVPlanarComponentInfo structure for each plane of the buffer.

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

struct CVPlanarComponentInfo

A structure for describing planar components.

struct CVPlanarPixelBufferInfo_YCbCrPlanar

A structure for describing YCbCr planar buffers.

struct CVPlanarPixelBufferInfo_YCbCrBiPlanar

A structure for describing YCbCr biplanar buffers.

