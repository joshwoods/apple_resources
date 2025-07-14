

- DeviceActivity
-  DeviceActivityName 

Structure

# DeviceActivityName

The unique name of an activity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
struct DeviceActivityName
```

## Overview

Use `DeviceActivityName` to associate an activity with some of your application’s data. It’s not possible to have multiple activities with the same name. Monitoring a second activity with the same name as a previous activity overwrites the schedule for the first one.

## Topics

### Creating an Instance

init(rawValue: String)

Creates a new instance with the specified raw value.

init(String)

Creates a new instance with the specified raw value.

var rawValue: String

The corresponding value of the raw type.

### Identifying and Comparing Errors

var hashValue: Int

The hash value.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two values aren’t equal.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable

## See Also

### Manage Activities

struct DeviceActivityEvent

An event that represents an application, category, or website activity.

struct DeviceActivitySchedule

A calendar-based schedule for when to monitor a device’s activity.

struct DeviceActivityCenter

A class that enables an application’s extension to start monitoring scheduled device activity.

