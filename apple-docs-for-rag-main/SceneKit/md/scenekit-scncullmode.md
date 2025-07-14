

- SceneKit
-  SCNCullMode 

Enumeration

# SCNCullMode

The modes SceneKit uses to determine which polygons to render in a surface, used by the cullMode property.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum SCNCullMode
```

## Overview

The vertex data and normal vectors in a geometry designate which side of each polygon is to be considered its front face, and the geometry’s orientation with respect to the camera determines which front surfaces are currently visible. Typically, back-facing surfaces are found only on the interior of a closed geometry, obscured by front-facing surfaces, so rendering these surfaces has a performance cost but no visible effect.

## Topics

### Enumeration Cases

case back

case front

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Customizing Rendered Appearance

var isLitPerPixel: Bool

A Boolean value that determines whether SceneKit performs lighting calculations per vertex or per pixel. Animatable.

var isDoubleSided: Bool

A Boolean value that determines whether SceneKit renders both front and back faces of a surface.

var cullMode: SCNCullMode

The mode determining which faces of a surface SceneKit renders. Animatable.

var fillMode: SCNFillMode

enum SCNFillMode

