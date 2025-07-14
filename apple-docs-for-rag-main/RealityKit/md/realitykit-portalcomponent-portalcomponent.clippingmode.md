

- RealityKit
- PortalComponent
-  PortalComponent.ClippingMode 

Enumeration

# PortalComponent.ClippingMode

Specifies the mode of clipping for a portal.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
enum ClippingMode
```

## Overview

This type can be passed into clippingMode to configure the portal component’s clipping feature.

With PortalComponent.ClippingMode.disabled, contents in portal world are not clipped

With PortalComponent.ClippingMode.plane(_:), contents within portal are clipped by the edge of the plane.

## Topics

### Operators

static func == (PortalComponent.ClippingMode, PortalComponent.ClippingMode) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case disabled

Disables clipping of the contents within the portal.

case plane(PortalComponent.Plane)

Clips the contents within the portal by the edge of the plane.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

