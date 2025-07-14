

- Foundation
- RunLoop
- RunLoop.Mode
-  default 

Type Property

# default

The mode set to handle input sources other than connection objects.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let `default`: RunLoop.Mode
```

## Discussion

This is the most commonly used run-loop mode.

## See Also

### System Run Loop Modes

static let common: RunLoop.Mode

A pseudo-mode that includes one or more other run loop modes.

static let eventTracking: RunLoop.Mode

The mode set when tracking events modally, such as a mouse-dragging loop.

static let modalPanel: RunLoop.Mode

The mode set when waiting for input from a modal panel, such as a save or open panel.

static let tracking: RunLoop.Mode

The mode set while tracking in controls takes place.

