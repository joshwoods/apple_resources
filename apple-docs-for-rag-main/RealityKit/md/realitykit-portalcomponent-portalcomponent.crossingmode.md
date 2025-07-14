

- RealityKit
- PortalComponent
-  PortalComponent.CrossingMode 

Enumeration

# PortalComponent.CrossingMode

Specifies the mode of crossing for a portal.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
enum CrossingMode
```

## Overview

You pass this type to crossingMode to configure the portal component’s crossing feature.

Use PortalComponent.CrossingMode.disabled to disallow contents within the portal to cross out of the portal boundary.

Use PortalComponent.CrossingMode.plane(_:) to allow contents within the portal world with a PortalCrossingComponent to cross out of this planar definition of the portal boundary.

## Topics

### Operators

static func == (PortalComponent.CrossingMode, PortalComponent.CrossingMode) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case disabled

Disallows contents within the portal to cross out of the portal boundary.

case plane(PortalComponent.Plane)

Allows contents within the portal to cross out of the portal along the provided plane.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

