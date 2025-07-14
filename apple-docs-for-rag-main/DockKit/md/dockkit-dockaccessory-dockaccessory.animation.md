

- DockKit
- DockAccessory
-  DockAccessory.Animation 

Enumeration

# DockAccessory.Animation

Character animations that describe how to move the dock accessory.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
enum Animation
```

## Overview

Each animation executes on a predefined trajectory. See animate(motion:) for more information.

## Topics

### Operators

static func == (DockAccessory.Animation, DockAccessory.Animation) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case kapow

The dock accessory performs a quick tilt and snaps back with some oscillation.

case no

The dock accessory traces a horizontal head shake.

case wakeup

The dock accessory moves upwards towards center.

case yes

The dock accessory traces a vertical head nod.

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
- Sendable

## See Also

### Performing animation

func animate(motion: DockAccessory.Animation) async throws -> Progress

Starts an animation sequence.

func setRegionOfInterest(CGRect) async throws

Sets the area in the video frame in which the dock accessory tracks a subject.

var regionOfInterest: CGRect

The area in the video frame in which the dock accessory tracks a subject.

