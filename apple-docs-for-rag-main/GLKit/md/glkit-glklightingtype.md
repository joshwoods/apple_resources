

- GLKit
-  GLKLightingType 

Enumeration

# GLKLightingType

A constant that describes how lighting is calculated by an effect.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
enum GLKLightingType
```

## Overview

Typically, per-pixel lighting should be enabled when it provides an improvement in image quality without greatly reducing your application’s performance. Calculating the lighting equation at each fragment greatly increases the number of calculations required to calculate the lighting for a scene. However, calculating lighting only at vertices sometimes produces unusual or inaccurate results, particularly when your application uses spotlights or specular highlighting. For example, when per-pixel lighting is disabled, a narrow spotlight projected at the center of a large triangle may disappear entirely because the vertices that define the triangle all lie outside the area covered by the spotlight. That same triangle, when rendered using per-pixel lighting, would be rendered correctly.

## Topics

### Constants

case perVertex

Indicates that the lighting calculations are performed at each vertex in a triangle and then interpolated across the triangle.

case perPixel

Indicates that the inputs to the lighting calculation are interpolated across a triangle and the lighting calculations are performed at each fragment.

### Initializers

init?(rawValue: GLint)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

