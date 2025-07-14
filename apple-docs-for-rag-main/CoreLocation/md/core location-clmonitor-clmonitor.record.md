

- Core Location
- CLMonitor
-  CLMonitor.Record 

Structure

# CLMonitor.Record

A structure that represents a condition and its associated event information that the framework is monitoring.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
struct Record
```

## Overview

The `CLMonitor.Record` contains a condition and most recent event that affects it.

## Topics

### Record characteristics

let condition: any CLCondition

The condition that the framework is monitoring for.

let lastEvent: CLMonitor.Event

The most recent event the monitor records.

## Relationships

### Conforms To

- Sendable

## See Also

### Monitor events

struct Event

An event object that the framework passes to the events sequence in the monitor.

struct Events

A type that represents an asynchronous sequence of events.

