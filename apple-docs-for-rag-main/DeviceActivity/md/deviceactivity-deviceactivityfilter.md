

- DeviceActivity
-  DeviceActivityFilter 

Structure

# DeviceActivityFilter

A type that filters the device activity data to include in a report.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
struct DeviceActivityFilter
```

## Overview

Your app can choose to filter device activity data for a specific date interval, filter by user and device, as well as specify a subset of applications, categories, and web domains to include in a report.

## Topics

### Structures

struct Devices

A type your app uses to indiciate which devices to include in a device activity report.

struct Users

A type your app uses to indicate which users to include in a device activity report.

### Operators

static func == (DeviceActivityFilter, DeviceActivityFilter) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(segment: DeviceActivityFilter.SegmentInterval, devices: DeviceActivityFilter.Devices?, applications: Set&lt;ApplicationToken>, categories: Set&lt;ActivityCategoryToken>, webDomains: Set&lt;WebDomainToken>)

Creates a new filter for the current user.

init(segment: DeviceActivityFilter.SegmentInterval, users: DeviceActivityFilter.Users, devices: DeviceActivityFilter.Devices, applications: Set&lt;ApplicationToken>, categories: Set&lt;ActivityCategoryToken>, webDomains: Set&lt;WebDomainToken>)

Creates a new filter for the specified users and devices.

### Instance Properties

var applications: Set&lt;ApplicationToken>

An optional set of applications to include in a report.

var categories: Set&lt;ActivityCategoryToken>

An optional set of categories to include in a report.

let devices: DeviceActivityFilter.Devices?

The devices to include in a report.

var segmentInterval: DeviceActivityFilter.SegmentInterval

The interval at which the system subdivides the report’s device activity data during a specified date interval.

let users: DeviceActivityFilter.Users?

The users to include in a report.

var webDomains: Set&lt;WebDomainToken>

An optional set of web domains to include in a report.

### Enumerations

enum SegmentInterval

A type indicating the interval at which the system subdivides device activity data within a specified date interval.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

