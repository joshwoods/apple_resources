

- DockKit
- DockAccessory
-  DockAccessory.BatteryState 

Structure

# DockAccessory.BatteryState

A struct that represents an accessory battery state.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
struct BatteryState
```

## Overview

This state is emitted when the battery level changes on accessory.

## Topics

### Operators

static func == (DockAccessory.BatteryState, DockAccessory.BatteryState) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

let batteryLevel: Double

Current charge percentage (0..1) of the battery

let chargeState: DockAccessory.BatteryChargeState

An enumeration representing the charge state of the battery

var hashValue: Int

The hash value.

let lowBattery: Bool

True when accessory deems its charge to be too low to function properly

let name: String

The name of the battery that is sending this state from accessory

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

