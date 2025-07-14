

- DeviceActivity
- DeviceActivityFilter
-  DeviceActivityFilter.Devices 

Structure

# DeviceActivityFilter.Devices

A type your app uses to indiciate which devices to include in a device activity report.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
struct Devices
```

## Overview

Users can control whether a device shares its data with other devices in their circle in iCloud settings.

## Topics

### Operators

static func == (DeviceActivityFilter.Devices, DeviceActivityFilter.Devices) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(Set&lt;DeviceActivityData.Device.Model>)

Filters data for the provided device models.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Properties

static let all: DeviceActivityFilter.Devices

Filters data for all devices that are sharing activity data with the current device.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable

