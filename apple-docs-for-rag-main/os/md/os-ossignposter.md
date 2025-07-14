

- os
-  OSSignposter 

Structure

# OSSignposter

An object for measuring task performance using the unified logging system.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
struct OSSignposter
```

## Mentioned in 

Recording Performance Data

## Overview

Signposts allow you to record meaningful information about the duration of your app’s tasks using the same subsystems and categories that you use for logging. Use `OSSignposter` to create signposted intervals in your code, and then use Instruments’ `os_signposts` instrument to record those intervals as you run your app and perform the actions to measure. Instruments displays signpost data visually in a timeline.

To add a signposted interval, create a signpost ID — an identifier that disambiguates intervals that have the same name, subsystem, and category, and that exist within the same scope — and then add a call to one of the class’s `beginInterval` methods just before the code you want to measure. Retain the interval state it returns, and end the interval by passing that state to one of the class’s `endInterval` methods, which you call immediately after the measured code. A signposter uses interval state to enforce a number of runtime assertions, the behavior of which depends on your app’s build configuration. For more information, see OSSignpostIntervalState. A signposted interval consists of one begin call and one end call only.

`OSSignposter` also provides functionality to signpost a closure, and to emit individual signposts that don’t have a duration that you can use to highlight points of interest, such as when the user taps a button or performs a specific gesture.

## Topics

### Creating a Signposter

init()

Creates a signposter that uses the default subsystem.

init(subsystem: String, category: String)

Creates a signposter that uses the specified subsystem and category.

init(subsystem: String, category: OSLog.Category)

Creates a signposter that uses the specified subsystem and system-defined log category.

init(logger: Logger)

Creates a signposter that uses the subsystem and category of an existing logger.

init(logHandle: OSLog)

Creates a signposter that uses the subsystem and category of an existing log.

static var disabled: OSSignposter

A shared signposter that doesn’t emit signposts at runtime.

### Getting State

var isEnabled: Bool

A Boolean value that indicates whether the signposter can emit signposts.

### Generating Signpost IDs

func makeSignpostID() -> OSSignpostID

Returns an identifier that’s unique within the scope of the signposter.

func makeSignpostID(from: AnyObject) -> OSSignpostID

Returns an identifier that the signposter derives from the specified object.

struct OSSignpostID

An identifier that disambiguates signposted intervals.

### Starting a Signposted Interval

func beginInterval(StaticString, id: OSSignpostID) -> OSSignpostIntervalState

Begins a signposted interval.

func beginInterval(StaticString, id: OSSignpostID, SignpostMetadata) -> OSSignpostIntervalState

Begins a signposted interval and attaches the specified message.

func beginAnimationInterval(StaticString, id: OSSignpostID) -> OSSignpostIntervalState

Begins a signposted interval for measuring an animation.

func beginAnimationInterval(StaticString, id: OSSignpostID, SignpostMetadata) -> OSSignpostIntervalState

Begins a signposted interval for measuring an animation, and attaches a message.

class OSSignpostIntervalState

An object that tracks the state of a signposted interval.

typealias SignpostMetadata

The type that represents a message you attach to a signpost.

### Stopping a Signposted Interval

func endInterval(StaticString, OSSignpostIntervalState)

Ends the signposted interval that corresponds to the specified name and state.

func endInterval(StaticString, OSSignpostIntervalState, SignpostMetadata)

Ends a signposted interval and attaches the specified message.

### Measuring a Closure

func withIntervalSignpost&lt;T>(StaticString, id: OSSignpostID, around: () throws -> T) rethrows -> T

Measures the execution of the specified closure.

func withIntervalSignpost&lt;T>(StaticString, id: OSSignpostID, SignpostMetadata, around: () throws -> T) rethrows -> T

Measures the execution of a closure and attaches the specified message.

### Emitting Individual Signposts

func emitEvent(StaticString, id: OSSignpostID)

Marks a point of interest in time.

func emitEvent(StaticString, id: OSSignpostID, SignpostMetadata)

Marks a point of interest in time and attaches the specified message.

## Relationships

### Conforms To

- Sendable

## See Also

### Measure Events

Recording Performance Data

Add signposts to record interesting time-based events.

Legacy Signpost Symbols

Migrate your code away from using these legacy symbols.

struct OSSignpostType

The different kinds of signpost.

Deprecated

typealias os_signpost_id_t

An identifier you use to distinguish between signposts that have the same name and destination log.

