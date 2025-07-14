

- DockKit
- DockAccessory
-  DockAccessory.AccessoryEvent 

Enumeration

# DockAccessory.AccessoryEvent

An enumeration that represents an accessory event.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+

``` source
enum AccessoryEvent
```

## Overview

This event propagates input from the dock accessory. Example events are button presses or requests for common camera controls.

## Topics

### Operators

static func == (DockAccessory.AccessoryEvent, DockAccessory.AccessoryEvent) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case button(id: Int, pressed: Bool)

A button press event on the dock accessory.

case cameraFlip

A camera flip event that indicates a request to switch between back and front cameras.

case cameraShutter

A camera shutter toggle event.

case cameraZoom(factor: Double)

A camera zoom event.

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

