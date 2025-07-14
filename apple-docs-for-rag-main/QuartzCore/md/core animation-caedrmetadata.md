

- Core Animation
-  CAEDRMetadata 

Class

# CAEDRMetadata

Metadata describing how extended dynamic range (EDR) values should be tone mapped.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 10.15+visionOS 1.0+

``` source
class CAEDRMetadata
```

## Overview

If you need specific tone-mapping behavior, set the edrMetadata property of a CAMetalLayer to point to an instance of this class.

## Topics

### Retrieving Hybrid-Log Gamma Metadata

class var hlg: CAEDRMetadata

Extended dynamic range (EDR) metadata for the Hybrid Log-Gamma (HLG) transfer function.

### Retrieving HDR10 Metadata

class func hdr10(displayInfo: Data?, contentInfo: Data?, opticalOutputScale: Float) -> CAEDRMetadata

Creates EDR metadata for HDR10 content based on mastering display color information and content light levels.

class func hdr10(minLuminance: Float, maxLuminance: Float, opticalOutputScale: Float) -> CAEDRMetadata

Creates EDR metadata for HDR10 content based on the luminance characteristics of a mastering display.

### Type Properties

class var isAvailable: Bool

### Type Methods

class func hlg(ambientViewingEnvironment: Data) -> CAEDRMetadata

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Metal and OpenGL

class CAMetalLayer

A Core Animation layer that Metal can render into, typically displayed onscreen.

protocol CAMetalDrawable

A Metal drawable associated with a Core Animation layer.

class CAEAGLLayer

A layer that supports drawing OpenGL content in iOS and tvOS applications.

Deprecated

class CAOpenGLLayer

A layer that provides a layer suitable for rendering OpenGL content.

Deprecated

class CARenderer

A layer that allows an application to render a layer tree into a Core OpenGL context.

