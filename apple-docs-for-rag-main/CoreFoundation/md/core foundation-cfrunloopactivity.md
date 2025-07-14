

- Core Foundation
-  CFRunLoopActivity 

Structure

# CFRunLoopActivity

Run loop activity stages in which run loop observers can be scheduled.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CFRunLoopActivity
```

## Overview

The run loop stages in which an observer is scheduled are selected when the observer is created with CFRunLoopObserverCreate(_:_:_:_:_:_:).

## Topics

### Constants

static var entry: CFRunLoopActivity

The entrance of the run loop, before entering the event processing loop. This activity occurs once for each call to CFRunLoopRun() and CFRunLoopRunInMode(_:_:_:).

static var beforeTimers: CFRunLoopActivity

Inside the event processing loop before any timers are processed.

static var beforeSources: CFRunLoopActivity

Inside the event processing loop before any sources are processed.

static var beforeWaiting: CFRunLoopActivity

static var afterWaiting: CFRunLoopActivity

Inside the event processing loop after the run loop wakes up, but before processing the event that woke it up. This activity occurs only if the run loop did in fact go to sleep during the current loop.

static var exit: CFRunLoopActivity

The exit of the run loop, after exiting the event processing loop. This activity occurs once for each call to CFRunLoopRun() and CFRunLoopRunInMode(_:_:_:).

static var allActivities: CFRunLoopActivity

A combination of all the preceding stages.

### Initializers

init(rawValue: CFOptionFlags)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

