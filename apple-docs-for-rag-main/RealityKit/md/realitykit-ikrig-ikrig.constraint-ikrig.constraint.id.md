

- RealityKit
- IKRig
- IKRig.Constraint
-  IKRig.Constraint.ID 

Structure

# IKRig.Constraint.ID

The identity type for a constraint in a rig.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct ID
```

## Overview

Note

Stable only during the lifetime of the containing process.

## Topics

### Operators

static func == (IKRig.Constraint.ID, IKRig.Constraint.ID) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable

