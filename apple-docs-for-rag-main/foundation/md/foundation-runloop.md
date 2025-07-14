

- Foundation
-  RunLoop 

Class

# RunLoop

The programmatic interface to objects that manage input sources.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class RunLoop
```

## Mentioned in 

Processing URL session data task results with Combine

## Overview

A RunLoop object processes input for sources, such as mouse and keyboard events from the window system and Port objects. A RunLoop object also processes Timer events.

Your application neither creates nor explicitly manages RunLoop objects. The system creates a RunLoop object as needed for each Thread object, including the application’s main thread. If you need to access the current thread’s run loop, use the class method current.

Note that from the perspective of RunLoop, Timer objects aren’t “input”—they’re a special type, and they don’t cause the run loop to return when they fire.

Warning

The RunLoop class is generally not thread-safe, and you must call its methods only within the context of the current thread. Don’t call the methods of a RunLoop object running in a different thread, which might cause unexpected results.

## Topics

### Accessing Run Loops and Modes

class var current: RunLoop

Returns the run loop for the current thread.

var currentMode: RunLoop.Mode?

The receiver’s current input mode.

func limitDate(forMode: RunLoop.Mode) -> Date?

Performs one pass through the run loop in the specified mode and returns the date at which the next timer is scheduled to fire.

class var main: RunLoop

Returns the run loop of the main thread.

func getCFRunLoop() -> CFRunLoop

Returns the receiver’s underlying doc://com.apple.documentation/documentation/corefoundation/cfrunloop-rht object.

struct Mode

Modes that a run loop operates in.

### Managing Timers

func add(Timer, forMode: RunLoop.Mode)

Registers a given timer with a given input mode.

### Managing Ports

func add(Port, forMode: RunLoop.Mode)

Adds a port as an input source to the specified mode of the run loop.

func remove(Port, forMode: RunLoop.Mode)

Removes a port from the specified input mode of the run loop.

### Running a Loop

func run()

Puts the receiver into a permanent loop, during which time it processes data from all attached input sources.

func run(mode: RunLoop.Mode, before: Date) -> Bool

Runs the loop once, blocking for input in the specified mode until a given date.

func run(until: Date)

Runs the loop until the specified date, during which time it processes data from all attached input sources.

func acceptInput(forMode: RunLoop.Mode, before: Date)

Runs the loop once or until the specified date, accepting input only for the specified mode.

### Scheduling and Canceling Tasks

func perform(() -> Void)

Schedules a block that the run loop invokes.

func perform(inModes: [RunLoop.Mode], block: () -> Void)

Schedules a block that the run loop invokes when it’s running in any of the specified modes.

func perform(Selector, target: Any, argument: Any?, order: Int, modes: [RunLoop.Mode])

Schedules the sending of a message on the receiver.

func cancelPerform(Selector, target: Any, argument: Any?)

Cancels the sending of a previously scheduled message.

func cancelPerformSelectors(withTarget: Any)

Cancels all outstanding ordered performs scheduled with a given target.

### Scheduling Combine Publishers

struct SchedulerTimeType

The scheduler time type that the run loop uses.

struct SchedulerOptions

A set of options that affect the operation of the run loop scheduler.

### Default Implementations

Scheduler Implementations

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Scheduler

## See Also

### Run Loop Scheduling

class Timer

A timer that fires after a certain time interval has elapsed, sending a specified message to a target object.

