

- DeviceActivity
- DeviceActivityData
-  DeviceActivityData.ActivitySegment 

Structure

# DeviceActivityData.ActivitySegment

Represents the user’s activity during a particular date interval.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
struct ActivitySegment
```

## Overview

This type contains all of the activity details for a particular user on a particular device during dateInterval.

## Topics

### Operators

static func == (DeviceActivityData.ActivitySegment, DeviceActivityData.ActivitySegment) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var categories: DeviceActivityResults&lt;DeviceActivityData.CategoryActivity>

The user’s categorized device activity during the activity segment.

var dateInterval: DateInterval

The date interval of the activity segment.

var firstPickup: Date?

The first time the user picked up the device during the activity segment.

var hashValue: Int

The hash value.

var longestActivity: DateInterval?

The date interval of the user’s longest activity session during the activity segment.

var totalActivityDuration: TimeInterval

The total activity during the activity segment.

var totalPickupsWithoutApplicationActivity: Int

The number of times the user picked up the device but did not use any applications.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable

