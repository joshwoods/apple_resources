

- AppKit
- NSTouch
-  NSTouch.Phase 

Structure

# NSTouch.Phase

The possible phases of a touch.

macOS 10.7+

``` source
struct Phase
```

## Overview

These constants are used by phase.

## Topics

### Creating a Touch Phase

init(rawValue: UInt)

Creates a new touch phase from the given raw value.

### Constants

static var began: NSTouch.Phase

A finger touched the device. Or, a resting touch transitioned to an active touch and resting touches are not wanted by the view hierarchy.

static var moved: NSTouch.Phase

A finger moved on the device.

static var stationary: NSTouch.Phase

A finger is touching the device, but hasn’t moved since the previous event.

static var ended: NSTouch.Phase

A finger was lifted from the screen. Or, an active touch transitioned to a resting touch and resting touches are not wanted by the view hierarchy.

static var cancelled: NSTouch.Phase

The system cancelled tracking for the touch, as when (for example) the window associated with the touch resigns key or is deactivated.

static var touching: NSTouch.Phase

Matches the began, moved, or stationary phases of a touch.

static var any: NSTouch.Phase

Matches any phase of a touch.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Using Touch Properties

var identity: any NSCopying &amp; NSObjectProtocol

The changes to a particular touch during its lifetime.

var phase: NSTouch.Phase

The current phase of the touch.

var normalizedPosition: NSPoint

The normalized position of the touch.

var isResting: Bool

The indicator for a resting touch.

