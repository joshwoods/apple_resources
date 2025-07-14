

- SceneKit
-  SCNPhysicsFieldScope 

Enumeration

# SCNPhysicsFieldScope

Options for defining the region of space affected by a physics field, used by the scope property.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
enum SCNPhysicsFieldScope
```

## Overview

You define a region of space for a field using the position of the node containing the field and the field’s halfExtent and usesEllipsoidalExtent properties. Then, you use the scope property to choose whether the field’s area of effect is the interior of this region or whether it is the entirety of scene space excluding this region.

## Topics

### Constants

case insideExtent

The field’s effect applies only to objects within the region of space defined by its position and extent.

case outsideExtent

The field’s effect applies only to objects outside the region of space defined by its position and extent.

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

### Constants

typealias SCNFieldForceEvaluator

The signature for a block that SceneKit calls to determine the effect of a custom field on an object.

