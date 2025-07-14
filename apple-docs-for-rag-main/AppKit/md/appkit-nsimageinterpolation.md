

- AppKit
-  NSImageInterpolation 

Enumeration

# NSImageInterpolation

Constants that specify the interpolation, or image smoothing, behavior used by the image interpolation property.

macOS

``` source
enum NSImageInterpolation
```

## Overview

Use these constants with the imageInterpolation property.

## Topics

### Constants

case `default`

Use the context’s default interpolation.

case none

No interpolation.

case low

Fast, low-quality interpolation.

case medium

Medium quality, slower than the low interpolation option.

case high

Highest quality, slower than the medium interpolation option.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring Rendering Options

var compositingOperation: NSCompositingOperation

The graphics context’s global compositing operation setting.

enum NSCompositingOperation

Constants that describe compositing operators in terms of source and destination images, each having an opaque and transparent region.

var imageInterpolation: NSImageInterpolation

A constant that specifies the graphics context’s interpolation, or image smoothing, behavior.

var shouldAntialias: Bool

A Boolean value that indicates whether the graphics context uses antialiasing.

var patternPhase: NSPoint

The amount to offset the pattern color when filling the graphics context.

