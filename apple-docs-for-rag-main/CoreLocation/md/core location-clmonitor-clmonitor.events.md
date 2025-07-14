

- Core Location
- CLMonitor
-  CLMonitor.Events 

Structure

# CLMonitor.Events

A type that represents an asynchronous sequence of events.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
struct Events
```

## Overview

Use this structure to access and iterate over the events the framework delivers.

## Topics

### Utility methods

struct Iterator

The type that allows iteration over the elements of the sequence.

## Relationships

### Conforms To

- AsyncSequence
- Sendable

## See Also

### Monitor events

struct Event

An event object that the framework passes to the events sequence in the monitor.

struct Record

A structure that represents a condition and its associated event information that the framework is monitoring.

