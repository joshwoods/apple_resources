

- SceneKit
-  SCNChamferMode 

Enumeration

# SCNChamferMode

Options for which edges of an extruded shape are chamfered, used by the chamferMode property.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
enum SCNChamferMode
```

## Overview

## Topics

### Constants

case both

Apply a chamfer to both front and back edges of the extruded shape.

case front

Apply a chamfer to only the front edge of the extruded shape.

case back

Apply a chamfer to only the back edge of the extruded shape.

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

### Chamfering a Shape

var chamferMode: SCNChamferMode

A constant specifying which ends of the extruded shape’s profile are chamfered.

var chamferProfile: UIBezierPath?

A path that determines the cross-sectional contour of each chamfered edge.

var chamferRadius: CGFloat

The width or depth of each chamfered edge. Animatable.

