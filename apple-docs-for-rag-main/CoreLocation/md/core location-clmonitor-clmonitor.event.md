

- Core Location
- CLMonitor
-  CLMonitor.Event 

Structure

# CLMonitor.Event

An event object that the framework passes to the events sequence in the monitor.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
struct Event
```

## Overview

The framework delivers these events to an asynchronous sequence in the monitor that your app processes.

## Topics

### Event states

var accuracyLimited: Bool

A Boolean value that indicates whether the app receives accuracy-limited location updates.

var authorizationDenied: Bool

A Boolean value that indicates whether the app has local authorization.

var authorizationDeniedGlobally: Bool

A Boolean value that indicates whether the app has system-wide authorization.

var authorizationRequestInProgress: Bool

var authorizationRestricted: Bool

A Boolean value that indicates whether the app can make authorization changes.

var conditionLimitExceeded: Bool

A Boolean value that indicates whether the app receives location updates based on other monitoring conditions.

var conditionUnsupported: Bool

A Boolean value that indicates whether the app receives location updates based on the supported condition.

var insufficientlyInUse: Bool

A Boolean value that indicates whether the app receives location updates because it’s insufficiently in use.

var persistenceUnavailable: Bool

A Boolean value that indicates whether it receives location updates based on successful persistence.

var serviceSessionRequired: Bool

### Event characteristics

var date: Date

A date indicating the time of the event.

var identifier: String

A string that identifies the event.

let refinement: (any CLCondition)?

An optional instance of a condition that represents the most specific condition that this event can apply to.

var state: CLMonitor.Event.State

The event’s state.

### Type aliases

typealias State

The type that represents the state of the monitoring event.

## Relationships

### Conforms To

- Sendable

## See Also

### Monitor events

struct Record

A structure that represents a condition and its associated event information that the framework is monitoring.

struct Events

A type that represents an asynchronous sequence of events.

