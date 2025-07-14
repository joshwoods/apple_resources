

- Foundation
- RunLoop
-  RunLoop.Mode 

Structure

# RunLoop.Mode

Modes that a run loop operates in.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct Mode
```

## Discussion

NSApplication defines additional run loop modes, including the following:

- modalPanel

- eventTracking

## Topics

### System Run Loop Modes

static let common: RunLoop.Mode

A pseudo-mode that includes one or more other run loop modes.

static let `default`: RunLoop.Mode

The mode set to handle input sources other than connection objects.

static let eventTracking: RunLoop.Mode

The mode set when tracking events modally, such as a mouse-dragging loop.

static let modalPanel: RunLoop.Mode

The mode set when waiting for input from a modal panel, such as a save or open panel.

static let tracking: RunLoop.Mode

The mode set while tracking in controls takes place.

### Run Loop Mode Creation

init(String)

Creates a run loop mode using the specified string value.

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

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

