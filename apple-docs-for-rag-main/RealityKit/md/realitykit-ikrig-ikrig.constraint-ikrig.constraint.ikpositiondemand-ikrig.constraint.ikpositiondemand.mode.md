

- RealityKit
- IKRig
- IKRig.Constraint
- IKRig.Constraint.IKPositionDemand
-  IKRig.Constraint.IKPositionDemand.Mode 

Enumeration

# IKRig.Constraint.IKPositionDemand.Mode

Describes the acting modes of positional demands.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
enum Mode
```

## Overview

See animationOverrideWeight for the actual target compute logic.

## Topics

### Operators

static func == (IKRig.Constraint.IKPositionDemand.Mode, IKRig.Constraint.IKPositionDemand.Mode) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case poleVector

A mode which pulls the joint in the direction of the set position target.

case reach

A mode which uses the set position target.

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

- Copyable
- Equatable
- Hashable

