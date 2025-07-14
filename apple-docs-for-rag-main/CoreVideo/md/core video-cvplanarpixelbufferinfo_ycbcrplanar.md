

- Core Video
-  CVPlanarPixelBufferInfo_YCbCrPlanar 

Structure

# CVPlanarPixelBufferInfo_YCbCrPlanar

A structure for describing YCbCr planar buffers.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
struct CVPlanarPixelBufferInfo_YCbCrPlanar
```

## Topics

### Initializers

init()

init(componentInfoY: CVPlanarComponentInfo, componentInfoCb: CVPlanarComponentInfo, componentInfoCr: CVPlanarComponentInfo)

### Properties

var componentInfoCb: CVPlanarComponentInfo

A CVPlanarComponentInfo structure containing information on the Cb component of the buffer.

var componentInfoCr: CVPlanarComponentInfo

A CVPlanarComponentInfo structure containing information on the Cr component of the buffer.

var componentInfoY: CVPlanarComponentInfo

A CVPlanarComponentInfo structure containing information on the Y component of the buffer.

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

struct CVPlanarPixelBufferInfo

A structure for describing planar buffers.

struct CVPlanarPixelBufferInfo_YCbCrBiPlanar

A structure for describing YCbCr biplanar buffers.

