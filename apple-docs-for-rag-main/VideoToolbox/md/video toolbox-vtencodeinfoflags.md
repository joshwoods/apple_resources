

- Video Toolbox
-  VTEncodeInfoFlags 

Structure

# VTEncodeInfoFlags

Flags that indicate encoder state.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.0+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
struct VTEncodeInfoFlags
```

## Topics

### Info Flags

static var asynchronous: VTEncodeInfoFlags

A flag that indicates that an encode operation ran asynchronously.

static var frameDropped: VTEncodeInfoFlags

A flag that indicates that a frame dropped during encoding.

### Initializers

init(rawValue: UInt32)

Creates a flags structure with a raw value.

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

class VTCompressionSession

A reference to a VideoToolbox compression session.

