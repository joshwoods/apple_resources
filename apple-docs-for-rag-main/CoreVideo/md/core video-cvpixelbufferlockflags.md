

- Core Video
-  CVPixelBufferLockFlags 

Structure

# CVPixelBufferLockFlags

The flags to pass to CVPixelBufferLockBaseAddress(_:_:) and CVPixelBufferUnlockBaseAddress(_:_:).

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
struct CVPixelBufferLockFlags
```

## Topics

### Constants

static var readOnly: CVPixelBufferLockFlags

A read-only buffer.

### Initializers

init(rawValue: CVOptionFlags)

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

### Data Types

typealias CVPixelBuffer

A reference to a Core Video pixel buffer object.

struct CVPlanarComponentInfo

A structure for describing planar components.

struct CVPlanarPixelBufferInfo

A structure for describing planar buffers.

struct CVPlanarPixelBufferInfo_YCbCrPlanar

A structure for describing YCbCr planar buffers.

struct CVPlanarPixelBufferInfo_YCbCrBiPlanar

A structure for describing YCbCr biplanar buffers.

