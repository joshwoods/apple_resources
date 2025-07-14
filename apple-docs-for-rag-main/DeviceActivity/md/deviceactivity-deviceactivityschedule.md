

- DeviceActivity
-  DeviceActivitySchedule 

Structure

# DeviceActivitySchedule

A calendar-based schedule for when to monitor a device’s activity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
struct DeviceActivitySchedule
```

## Overview

Create a new schedule using `DateComponents` that allows your app to monitor the person’s device activity during a period of time. You can set a schedule for your app to monitor on a regularly occuring basis. You can create a warning time that the system uses to provide your app extension with callbacks whenever a schedule is about to start or end, or when an event is close to reaching its threshold.

## Topics

### Creating a Schedule

init(intervalStart: DateComponents, intervalEnd: DateComponents, repeats: Bool, warningTime: DateComponents?)

Creates a new schedule.

var intervalEnd: DateComponents

The date components that represent the end time for a schedule’s interval.

var intervalStart: DateComponents

The date components that represent the start time for a schedule’s interval.

var nextInterval: DateInterval?

The schedule’s next interval or the current interval if one is ongoing.

var repeats: Bool

A Boolean value that indicates whether the schedule recurs.

var warningTime: DateComponents?

Optional components that generate a warning prior to regularly scheduled events.

### Comparing Schedules

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two values aren’t equal.

static func == (DeviceActivitySchedule, DeviceActivitySchedule) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

## See Also

### Manage Activities

struct DeviceActivityEvent

An event that represents an application, category, or website activity.

struct DeviceActivityName

The unique name of an activity.

struct DeviceActivityCenter

A class that enables an application’s extension to start monitoring scheduled device activity.

