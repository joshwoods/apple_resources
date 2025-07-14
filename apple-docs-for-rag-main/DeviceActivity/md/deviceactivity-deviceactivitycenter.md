

- DeviceActivity
-  DeviceActivityCenter 

Structure

# DeviceActivityCenter

A class that enables an application’s extension to start monitoring scheduled device activity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
struct DeviceActivityCenter
```

## Overview

Activity begins when someone first uses a device within the scheduled time interval and ends when someone first uses the device outside of the interval. The system only invokes the intervalDidStart(for:) and intervalDidEnd(for:) when the device is in use. Likewise, the system invokes the eventDidReachThreshold(_:activity:) function when an event reaches its threshold.

## Topics

### Monitoring Device Activities

init()

Creates an activity center to manage which device activities your application monitors.

func startMonitoring(DeviceActivityName, during: DeviceActivitySchedule, events: [DeviceActivityEvent.Name : DeviceActivityEvent]) throws

Starts monitoring the specified device activity.

func stopMonitoring([DeviceActivityName])

Stops monitoring the specified device activities.

var activities: [DeviceActivityName]

The activities that the application’s extension currently monitors.

### Getting the Events and Schedules

func events(for: DeviceActivityName) -> [DeviceActivityEvent.Name : DeviceActivityEvent]

Fetches the events of a device activity.

func schedule(for: DeviceActivityName) -> DeviceActivitySchedule?

Fetches the schedule of a device activity.

### Enumerations

enum MonitoringError

Errors that may occur when starting to monitor an activity.

## See Also

### Manage Activities

struct DeviceActivityEvent

An event that represents an application, category, or website activity.

struct DeviceActivityName

The unique name of an activity.

struct DeviceActivitySchedule

A calendar-based schedule for when to monitor a device’s activity.

