

- DeviceActivity
-  DeviceActivityEvent 

Structure

# DeviceActivityEvent

An event that represents an application, category, or website activity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
struct DeviceActivityEvent
```

## Overview

Device activity is the amount of time an application, category, or web domain is frontmost on the screen and accumulates based on the time zone of the scheduled start date. Web domain activity includes domains visited in Safari or any third-party browser that contributes web usage via a `STWebpageController`.

## Topics

### Creating an Event

init(applications: Set&lt;ApplicationToken>, categories: Set&lt;ActivityCategoryToken>, webDomains: Set&lt;WebDomainToken>, threshold: DateComponents)

Creates a new event.

struct Name

The unique name of an event.

var includesAllActivity: Bool

A Boolean value that indicates whether the event includes all applications, categories, and web domains.

### Including Objects in an Event

var applications: Set&lt;ApplicationToken>

The applications that the event includes.

var categories: Set&lt;ActivityCategoryToken>

The categories that the event includes.

var webDomains: Set&lt;WebDomainToken>

The web domains that the event includes.

var threshold: DateComponents

The amount of time to monitor the provided applications, categories, and web domains.

### Comparing Events and Schedules

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two values aren’t equal.

static func == (DeviceActivityEvent, DeviceActivityEvent) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(applications: Set&lt;ApplicationToken>, categories: Set&lt;ActivityCategoryToken>, webDomains: Set&lt;WebDomainToken>, threshold: DateComponents, includesPastActivity: Bool)

Creates a new event.

### Instance Properties

var includesPastActivity: Bool

Whether the system takes into account the person’s device activity before your app starts monitoring the event.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

## See Also

### Manage Activities

struct DeviceActivityName

The unique name of an activity.

struct DeviceActivitySchedule

A calendar-based schedule for when to monitor a device’s activity.

struct DeviceActivityCenter

A class that enables an application’s extension to start monitoring scheduled device activity.

