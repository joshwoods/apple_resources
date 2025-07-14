

- Core Location
-  CLMonitor 

Class

# CLMonitor

An object that monitors the conditions you add to it.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
actor CLMonitor
```

## Mentioned in 

Handling location updates in the background

## Overview

Use `CLMonitor` to monitor for and observe events such as the entry to a specific geographic area or proximity to a beacon with characteristics that you specify.

This service is unavailable in a compatible iPad or iPhone app running in visionOS.

## Topics

### Creating a monitor

init(String) async

Creates a location monitor with the name you specify.

### Adding and removing conditions

func add(any CLCondition, identifier: String)

Adds the given condition for monitoring.

func add(any CLCondition, identifier: String, assuming: CLMonitor.Event.State)

Adds the monitoring condition with the identifier and initial state you specify.

func record(for: String) -> CLMonitor.Record?

A record that contains a condition and the most recent event your app receives.

func remove(String)

Removes the condition and its enclosed record associated with the identifier you provide.

### Accessing the location monitor’s identifiers

var identifiers: [String]

An array that contains the identifiers of the conditions the framework is monitoring.

### Accessing the monitor’s events

let events: CLMonitor.Events

An asynchronous sequence of events that represent the conditions the monitor object observes.

### Monitor conditions

struct BeaconIdentityCondition

A condition that describes the characteristics of a beacon.

struct CircularGeographicCondition

A condition that describes a circular geographic area that a center point and radius define.

### Monitor events

struct Event

An event object that the framework passes to the events sequence in the monitor.

struct Record

A structure that represents a condition and its associated event information that the framework is monitoring.

struct Events

A type that represents an asynchronous sequence of events.

## Relationships

### Conforms To

- Actor
- Sendable

